# AI Writer Prompts Documentation

This document contains all AI prompts used in the AI Writer module. Use this as a reference to understand and improve the content generation.

**OpenAI Model:** `gpt-5.2-2025-12-11` (configured in `.env` as `OPENAI_DEFAULT_MODEL`)

---

## 1. Continue Writing Enhanced (`/api/writer/ai/continue-enhanced`)

**Purpose:** Continue writing content naturally based on existing content with full context.

**Context Included:** ✅ Voice | ✅ Keywords | ✅ Excluded Words | ✅ Format Guidelines | ✅ SERP Data

**Prompt Template:**
```
Continue writing the following content naturally in continuance from previously written content. Write up to 100 words.

[TONE/VOICE - if provided:]
Write in this style: {voice_instruction}
OR
Write in a {tone} tone.

[KEYWORDS - if provided:]
Naturally incorporate these SEO keywords into your content: {keywords}

[EXCLUDED WORDS - if provided:]
**IMPORTANT: Do NOT use these words or phrases in your writing:** {excluded_words}

[FORMAT GUIDELINES - if provided:]
Follow these guidelines: {format_guidelines}

[SERP CONTEXT - if provided:]
Top-ranking content averages {avg_word_count} words. Write comprehensive, valuable content.

Current content:
{content (last 3000 chars)}

Continue writing seamlessly from where the content left off. You may include new sections (## for H2, ### for H3) or paragraphs as appropriate. Use proper markdown formatting.
Output ONLY the continuation, no explanations or meta-commentary.
```

**Key Parameters:**
- `content`: Current document content (last 3000 chars for context)
- `keywords`: SEO keywords to incorporate (up to 30)
- `voice_instruction`: Brand voice style instructions
- `excluded_words`: Words/phrases AI should NOT use
- `format_guidelines`: Content formatting rules
- `serp_data`: Competitor analysis data (avg word count)

---

## 2. AI Write with Instruction (`/api/writer/ai/write`)

**Purpose:** Generate content based on user's specific instruction.

**Context Included:** ✅ Voice | ✅ Keywords | ✅ Excluded Words | ✅ SERP Data

**Prompt Template:**
```
You are an expert content writer. Based on the user's instruction, write high-quality content.

[VOICE - if provided:]
Write in this style: {voice_instruction}

[KEYWORDS - if provided:]
Naturally incorporate these SEO keywords: {keywords}

[EXCLUDED WORDS - if provided:]
**IMPORTANT: Do NOT use these words/phrases:** {excluded_words}

[SERP CONTEXT - if provided:]
Top-ranking content averages {avg_word_count} words.

User instruction: {instruction}

Context (existing content):
{content (first 2000 chars) OR "No existing content"}

Write the requested content up to 200 words or as user requested. Use HTML formatting (h2, h3, p, ul, li tags). Output ONLY the content, no explanations.
```

---

## 3. Transform Content (`/api/writer/ai/transform`)

**Purpose:** Transform selected content (expand, shorten, rephrase, etc.)

**Context Included:** ✅ Voice | ✅ Keywords | ✅ Excluded Words

**Prompt Template:**
```
Transform the following content according to the instruction.

[VOICE - if provided:]
Write in this style: {voice_instruction}

[KEYWORDS - if provided:]
Naturally incorporate these keywords if relevant: {keywords}

[EXCLUDED WORDS - if provided:]
**IMPORTANT: Do NOT use these words or phrases:** {excluded_words}

Instruction: {instruction}

Content to transform:
{content}

Output ONLY the transformed content in markdown format. Do not use HTML tags. Do not add explanations.
```

**Common Transform Instructions:**
- "Expand this section with more details"
- "Make this more concise"
- "Rephrase in a more professional tone"
- "Add examples to illustrate the points"
- "Convert to bullet points"

---

## 4. Generate Outline (`/api/writer/ai/generate-outline`)

**Purpose:** Create a comprehensive blog outline with detailed writing instructions for each section.

**Context Included:** ✅ SERP Data | ✅ Tone

**Prompt Template:**
```
Write a comprehensive blog outline for the keyword: "{keyword}"

[SERP CONTEXT - if provided:]
Top-ranking content analysis:
1. {title} ({word_count} words)
   Headings: {headings}
...

[TONE - if provided:]
Write in a {tone} tone.

Create the outline with detailed writing instructions for each section. Use this exact format:

## Introduction
- Write 2-3 compelling hook sentences about {keyword}
- Describe the main problem or need that {keyword} addresses
- Preview what readers will learn in this article
- Include a transition to the main content

## Key Takeaways
- [Key point 1 - what readers will learn about {keyword}]
- [Key point 2 - main benefit or outcome]
- [Key point 3 - important insight or statistic]
- [Key point 4 - actionable takeaway they can implement]

## [H2 Section Title 1 - What is {keyword}?]
- Define {keyword} in simple terms
- Explain why it matters to the reader
- Include relevant statistics or data points
- Add a real-world example or case study

### [H3 Subsection - Key Components]
- List the main components or elements
- Explain each briefly with bullet points
- Include practical examples

## [H2 Section Title 2 - Benefits/Advantages]
- List 3-5 main benefits with explanations
- Include data or research to support claims
- Add user testimonials or case studies if relevant

## [H2 Section Title 3 - How To / Step-by-Step Guide]
- Break down into numbered steps
- Include tips for each step
- Add warnings or common mistakes to avoid

## [H2 Section Title 4 - Best Practices / Tips]
- List 5-7 actionable tips
- Explain the "why" behind each tip

## [H2 Section Title 5 - Common Mistakes to Avoid]
- List 3-5 common pitfalls
- Explain consequences and solutions

## FAQs About {keyword}
- Include 3-5 common questions
- Provide concise, helpful answers

## Conclusion: Final Thoughts
- Summarize the 3 most important points
- Restate the main benefit to the reader
- Include a clear call to action
- End with an encouraging statement

Create 5-8 H2 sections with relevant H3 subsections. Each section instruction tells the writer exactly what to include.
```

---

## 5. Simple Continue (`/api/writer/ai/continue`)

**Purpose:** Basic content continuation with voice and keyword support.

**Context Included:** ✅ Voice | ✅ Keywords | ✅ Excluded Words

**Prompt Template:**
```
Continue writing the following content in the same style and tone in continuance from previously written. Write the next 50-100 words. You may include new sections (H2, H3) or paragraphs as appropriate.

[VOICE - if provided:]
Write in this style: {voice_instruction}

[KEYWORDS - if provided:]
Naturally incorporate these SEO keywords: {keywords}

[EXCLUDED WORDS - if provided:]
**IMPORTANT: Do NOT use these words/phrases:** {excluded_words}

Current content:
{content (last 2000 chars)}

Continue writing naturally from where the content left off. Output ONLY the continuation, no explanations. Use HTML formatting (h2, h3, p tags).
```

---

## 6. Generate Full Article (`/api/writer/ai/generate-article`)

**Purpose:** Generate a complete article from outline.

**Parameters:**
- `use_thinking_model: True` - Uses more advanced reasoning model
- Processes outline sections sequentially

---

## Brand Voice Integration

Brand voice is applied to all writing commands through the `voice_instruction` parameter. This should contain a 1200-1500 character description of the writing style including:

- **Tone:** formal, casual, humorous, authoritative
- **Voice Style:** confident, playful, empathetic
- **Diction:** simple, complex, technical
- **Formality Level:** formal, informal, balanced
- **Perspective:** first-person, second-person, third-person
- **Example Excerpts:** Sample content pieces

---

## Excluded Words Feature

The `excluded_words` parameter accepts a list of words or phrases that the AI should NOT use in generated content. This is useful for:

- Avoiding overused terms
- Excluding competitor brand names
- Removing clichés or buzzwords
- Maintaining brand consistency

**Example:** `["synergy", "leverage", "revolutionary", "game-changer"]`

---

## OpenAI Model Configuration

**Models Used:**
- `settings.OPENAI_DEFAULT_MODEL` - Default model (gpt-4o)
- `settings.OPENAI_REASONING_MODEL` - For complex tasks (gpt-4o)
- `settings.OPENAI_FAST_MODEL` - For quick responses (gpt-4o-mini)

**Note:** The system prompt mentions "GPT-5.2" and "GPT-5.1" but these are placeholder names. The actual models used are configured in `.env` via:
- `OPENAI_DEFAULT_MODEL`
- `OPENAI_REASONING_MODEL`

---

## Improving Prompts

To improve content generation:

1. **Add more context** - Include SERP data and competitor analysis
2. **Use brand voice** - Always provide voice_instruction for consistent tone
3. **Specify keywords** - Include target SEO keywords
4. **Set excluded words** - Remove unwanted terms
5. **Format guidelines** - Provide structure expectations

---

*Last Updated: December 27, 2025*
