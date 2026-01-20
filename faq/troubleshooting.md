# 🔧 Troubleshooting Guide

Solutions to common issues and technical problems.

---

## 🚨 Account & Login Issues

### Can't Log In

**Issue:** Login fails or shows error

**Solutions:**

✅ **Check credentials:**
- Verify email address is correct
- Password is case-sensitive
- Clear browser cache and cookies

✅ **Reset password:**
1. Click "Forgot Password"
2. Check email (including spam folder)
3. Follow reset link
4. Create new password

✅ **Google Sign-In issues:**
- Enable pop-ups for copyrocket.ai
- Try incognito/private mode
- Clear browser cache
- Use different browser

✅ **Account locked:**
- Too many failed attempts = temporary lock
- Wait 15 minutes and try again
- Contact support if persists

---

### Email Verification Not Received

**Issue:** Didn't get verification email after signup

**Solutions:**

✅ **Check spam/junk folder** - Most common issue

✅ **Wait 5-10 minutes** - Sometimes delayed

✅ **Check email address:**
- Verify spelling is correct
- No extra spaces

✅ **Resend verification:**
- Login attempt will prompt resend
- Or contact support

✅ **Try different email:**
- Some email providers block automated emails
- Use Gmail or Outlook

---

## 🔗 Google Search Console Issues

### Can't Connect GSC Property

**Issue:** Authorization fails or no properties shown

**Solutions:**

✅ **Verify GSC access:**
1. Visit [Google Search Console](https://search.google.com/search-console)
2. Confirm you see your properties
3. Check permission level (need Owner or Full User)

✅ **Use correct Google account:**
- Sign out of all Google accounts
- Sign in to GSC account first
- Then connect to Copyrocket AI

✅ **Pop-up blockers:**
- Enable pop-ups for copyrocket.ai
- Disable browser extensions temporarily
- Try different browser

✅ **Clear cookies:**
- Clear browser cache and cookies
- Close all browser tabs
- Start fresh connection

---

### GSC Data Not Showing

**Issue:** Connected but dashboard is empty

**Solutions:**

✅ **Wait for initial sync:**
- Takes 5-10 minutes after connection
- Refresh page after waiting

✅ **Check date range:**
- Try "Last 3 months" instead of "Last 7 days"
- New sites may have limited data

✅ **Verify property has data:**
- Check Google Search Console directly
- Confirm data exists for selected period
- GSC requires minimum traffic threshold

✅ **Reconnect property:**
1. Go to Properties page
2. Disconnect property
3. Wait 1 minute
4. Reconnect

✅ **Check GSC API status:**
- Verify Google Search Console API is not down
- Check [Google Status Dashboard](https://www.google.com/appsstatus)

---

### Data Doesn't Match GSC

**Issue:** Numbers different from Google Search Console

**This is normal because:**

**Google delays:**
- GSC data has 2-3 day lag
- Copyrocket AI shows most recent available

**Filtering differences:**
- We may filter spam queries
- Anonymous queries excluded
- Different aggregation methods

**Acceptable variance:** ±5%

**If variance is large (>10%):**
- Check same date range
- Verify same property selected
- Try manual refresh
- Contact support with screenshots

---

## 🤖 AI Chat Issues

### AI Chat Not Responding

**Issue:** Message sent but no response

**Solutions:**

✅ **Check internet connection:**
- Verify you're online
- Try refreshing page

✅ **Browser issues:**
- Clear cache and cookies
- Try different browser
- Disable extensions
- Update browser

✅ **Server status:**
- Check if service is experiencing issues
- Try again in a few minutes

✅ **Message too long:**
- Break into smaller questions
- Simplify your request

✅ **Quota exceeded (Free plan):**
- Check usage limits
- Upgrade to Premium
- Wait for monthly reset

---

### Agentic Search Takes Forever

**Issue:** Agentic search running too long (>2 minutes)

**Solutions:**

✅ **This is normal for deep research:**
- 30-60 seconds is typical
- Reading 30 URLs takes time
- Be patient

✅ **If stuck over 2 minutes:**
- Refresh page
- Try again without agentic search
- Simplify question
- Report to support

✅ **Optimize future searches:**
- Be more specific with questions
- Disable agentic for simple queries
- Use it only for strategic questions

---

### AI Responses Are Inaccurate

**Issue:** AI gives wrong information

**Solutions:**

✅ **Verify correct property:**
- Check property selector
- Data from wrong site?

✅ **Check date range:**
- Confirm selected period
- Try broader range

✅ **Rephrase question:**
- Be more specific
- Break complex questions into parts
- Provide more context

✅ **Cross-reference data:**
- Compare with GSC directly
- Verify in multiple reports

✅ **Report persistent issues:**
- Screenshot the issue
- Note your question
- Contact support

---

### Can't Upload Files

**Issue:** File upload fails or hangs

**Solutions:**

✅ **Check file size:**
- Maximum 10MB per file
- Compress large files
- Split into multiple uploads

✅ **Verify file type:**
- Supported: PDF, TXT, CSV, DOCX
- Not supported: EXE, ZIP, RAR

✅ **Browser issues:**
- Try different browser
- Disable extensions
- Clear cache

✅ **Internet connection:**
- Slow upload? Wait longer
- Check connection stability
- Try smaller file first

---

## 📊 Dashboard & Reports Issues

### Dashboard Not Loading

**Issue:** Blank page or infinite loading

**Solutions:**

✅ **Refresh page:**
- Hard refresh: Ctrl+Shift+R (Cmd+Shift+R on Mac)
- Clear cache if needed

✅ **Check browser:**
- Update to latest version
- Try different browser
- Disable extensions

✅ **Clear browser data:**
1. Clear cache and cookies
2. Close all tabs
3. Restart browser
4. Try again

✅ **Check internet:**
- Verify stable connection
- Try different network
- Disable VPN if using

✅ **Server status:**
- Wait 5 minutes
- Try again
- Contact support if persists

---

### Reports Showing Old Data

**Issue:** Data not updating or showing old information

**Solutions:**

✅ **Force refresh:**
- Click refresh icon on report
- Wait for sync to complete

✅ **Check sync status:**
- Look for "Last synced" timestamp
- If old, trigger manual refresh

✅ **GSC data delay:**
- Remember: GSC has 2-3 day delay
- Latest data may not be available yet

✅ **Clear local cache:**
- Log out and log back in
- Clear browser cache
- Should fetch fresh data

---

### Graphs Not Displaying

**Issue:** Charts missing or showing errors

**Solutions:**

✅ **Browser compatibility:**
- Update browser to latest version
- Chrome works best
- Safari/Firefox should work too

✅ **JavaScript enabled:**
- Verify JS is not blocked
- Disable script blockers
- Check browser settings

✅ **Ad blockers:**
- Temporarily disable
- Whitelist copyrocket.ai
- Test if graphs load

✅ **Insufficient data:**
- Need minimum data points
- Try longer date range
- Check if property has traffic

---

## ⚡ Performance Issues

### Site Running Slow

**Issue:** Copyrocket AI loading slowly

**Solutions:**

✅ **Check your internet:**
- Test speed at speedtest.net
- Need at least 5 Mbps
- Try different network

✅ **Clear browser cache:**
- Settings > Privacy > Clear data
- Clear last 7 days
- Restart browser

✅ **Close other tabs:**
- Too many tabs = slow performance
- Close unnecessary tabs
- Restart browser

✅ **Disable extensions:**
- Extensions can slow things down
- Disable ad blockers temporarily
- Try incognito mode

✅ **Update browser:**
- Use latest version
- Chrome 90+ recommended

✅ **Check system resources:**
- Close other programs
- Free up RAM
- Restart computer

---

### Images Not Loading

**Issue:** Generated images or UI images not showing

**Solutions:**

✅ **Check internet connection:**
- Images require good connection
- Try refreshing

✅ **Browser cache:**
- Clear cached images
- Hard refresh page

✅ **Content blockers:**
- Disable ad blockers
- Disable privacy extensions
- Whitelist our CDN

✅ **Regenerate images:**
- For AI-generated images, try again
- May have been generation error

---

## 🔧 Feature-Specific Issues

### Keyword Research Not Working

**Issue:** Research returns no results or errors

**Solutions:**

✅ **Check inputs:**
- Seed keyword entered?
- Location selected?
- Language selected?

✅ **Keyword too specific:**
- Try broader terms
- Check spelling
- Remove special characters

✅ **Quota exceeded:**
- Free plan has limits
- Check usage in dashboard
- Upgrade to Premium

✅ **API issues:**
- Try again in 5 minutes
- Different keyword
- Contact support if persists

---

### Autoblogging Not Generating Topics

**Issue:** Agent active but no topics generated

**Solutions:**

✅ **Check agent status:**
- Agent activated? (not paused)
- Schedule configured?
- Keywords provided?

✅ **Review configuration:**
- Niche too narrow?
- Add more keywords
- Broaden topic scope

✅ **Wait for schedule:**
- Topics generate based on schedule
- Daily agents: wait 24 hours
- Check "Last run" timestamp

✅ **Quota limits:**
- Premium feature
- Check subscription status
- Verify payment processed

---

### WordPress Integration Not Working

**Issue:** Can't connect WordPress or auto-publish fails

**Solutions:**

✅ **Verify WordPress credentials:**
- Correct URL (with https://)
- Valid username
- Application password (not regular password)

✅ **Check WordPress requirements:**
- WordPress 5.0+
- REST API enabled
- XML-RPC enabled
- No security plugins blocking API

✅ **Test connection:**
- Click "Test Connection"
- Review error message
- Fix indicated issue

✅ **Firewall/Security:**
- Whitelist Copyrocket AI IP
- Check security plugins (Wordfence, etc.)
- Contact host if API blocked

---

## 💳 Billing Issues

### Payment Failed

**Issue:** Card declined or payment error

**Solutions:**

✅ **Check card details:**
- Correct card number
- Valid expiration date
- Correct CVV
- Billing address matches

✅ **Contact bank:**
- Verify international transactions allowed
- Check for fraud holds
- Confirm sufficient funds

✅ **Try different payment method:**
- Different card
- Use PayPal
- Contact support for alternatives

✅ **Clear browser cache:**
- Cache issues can cause payment errors
- Try incognito mode

---

### Can't Cancel Subscription

**Issue:** Cancellation not working

**Solutions:**

✅ **Use account settings:**
1. Go to Settings > Subscription
2. Click "Cancel Subscription"
3. Follow prompts
4. Confirm cancellation

✅ **Email support:**
- Send to: support@copyrocket.ai
- Include account email
- Request cancellation
- We'll process within 24 hours

✅ **PayPal subscriptions:**
- May need to cancel in PayPal
- Log into PayPal
- Go to Settings > Payments > Manage automatic payments
- Find Copyrocket AI and cancel

---

### Didn't Receive Refund

**Issue:** Refund requested but not received

**Solutions:**

✅ **Check refund timeline:**
- 5-7 business days to process
- 7-10 days to appear in account
- Depends on bank/card issuer

✅ **Verify request:**
- Check email confirmation
- Contact support to verify status

✅ **Check payment method:**
- Refund goes to original payment method
- Credit card vs PayPal
- Bank statement may show pending

✅ **Contact support:**
- If 14+ days passed
- Provide transaction details
- We'll investigate

---

## 🌐 Browser-Specific Issues

### Chrome Issues

**Common Chrome problems:**

✅ **Extensions interfering:**
- Disable all extensions
- Test in incognito mode
- Re-enable one by one

✅ **Hardware acceleration:**
- Settings > Advanced > System
- Toggle "Use hardware acceleration"
- Restart Chrome

✅ **Clear Chrome data:**
- Settings > Privacy > Clear browsing data
- Select "All time"
- Check all boxes

---

### Safari Issues

**Common Safari problems:**

✅ **Cross-site tracking:**
- Settings > Privacy
- Disable "Prevent cross-site tracking"
- For copyrocket.ai

✅ **Clear Safari cache:**
- Develop > Empty Caches
- Or History > Clear History

✅ **Third-party cookies:**
- Preferences > Privacy
- Allow cookies from websites I visit

---

### Firefox Issues

**Common Firefox problems:**

✅ **Enhanced tracking protection:**
- Click shield icon in address bar
- Turn off for copyrocket.ai

✅ **Clear Firefox data:**
- Options > Privacy & Security
- Clear Data
- Check all boxes

✅ **Disable strict mode:**
- about:config
- privacy.trackingprotection.enabled = false

---

## 📱 Mobile Issues

### Mobile App Not Available

**Note:** Copyrocket AI is a web app, not a native mobile app.

**Access on mobile:**
- Open in mobile browser (Chrome, Safari)
- Fully responsive design
- All features available
- Bookmark for easy access

**For better mobile experience:**
- Add to home screen
- Use landscape mode for complex features
- Use desktop for intensive work

---

### Mobile Display Issues

**Issue:** Layout broken on mobile

**Solutions:**

✅ **Rotate device:**
- Some features better in landscape
- Tables need horizontal space

✅ **Update browser:**
- Use latest mobile browser
- Chrome or Safari recommended

✅ **Clear mobile cache:**
- Settings > Browser > Clear data

✅ **Zoom level:**
- Reset zoom to 100%
- Don't pinch zoom

---

## 🆘 Getting More Help

### When to Contact Support

Contact us if:
- ❌ Issue persists after trying solutions
- ❌ Error messages you don't understand
- ❌ Data loss or corruption
- ❌ Billing problems
- ❌ Security concerns
- ❌ Feature not working as documented

### How to Contact Support

**📧 Email:** support@copyrocket.ai

**🎫 Support Ticket:**
1. Click "Support" in sidebar
2. Click "New Ticket"
3. Describe issue
4. Attach screenshots
5. Submit

**💬 Live Chat:**
- Available for Premium users
- Business hours: 9 AM - 5 PM EST
- Click chat widget

### What to Include in Support Request

**Essential information:**
- 📧 Account email
- 🖥️ Browser and version
- 💻 Operating system
- 📸 Screenshots of issue
- 📝 Steps to reproduce
- ⚠️ Error messages (exact text)
- ⏰ When issue started
- 🔄 What you've tried already

**Better reports = Faster solutions!**

---

## 📋 Quick Troubleshooting Checklist

Before contacting support, try:

- [ ] Refresh page (Ctrl+Shift+R / Cmd+Shift+R)
- [ ] Clear browser cache and cookies
- [ ] Try different browser
- [ ] Try incognito/private mode
- [ ] Disable browser extensions
- [ ] Check internet connection
- [ ] Wait 5 minutes and try again
- [ ] Check account status/subscription
- [ ] Verify correct property/settings selected
- [ ] Check service status page

---

<div align="center">
  <p><strong>Most issues resolve with a simple refresh or cache clear! 🔧</strong></p>
  <p><a href="./general.md">← Back to FAQ</a> | <a href="../README.md">Documentation Home</a></p>
</div>
