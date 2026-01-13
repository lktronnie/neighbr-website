# Content Editing Locations Guide
## Quick Reference for Finding & Editing Website Text

**Last Updated:** January 13, 2026

This guide shows you **exactly where** to find and edit every piece of text on the Neighbr website.

---

## 📋 Table of Contents

1. [Navigation & Hero](#navigation--hero) ← **Edit in content.json**
2. [Product Features](#product-features) ← **Edit in pitch.html**
3. [Challenge Section](#challenge-section) ← **Edit in pitch.html**
4. [Get Started Section](#get-started-section) ← **Edit in pitch.html**
5. [Tenant Onboarding](#tenant-onboarding) ← **Edit in pitch.html**
6. [App Mockups](#app-mockups) ← **Edit in pitch.html**
7. [Trust & Security](#trust--security) ← **Edit in pitch.html**
8. [Contact Form](#contact-form) ← **Edit in pitch.html**
9. [Footer](#footer) ← **Edit in pitch.html**

---

## 🎯 Quick Reference: What's Where

| Section | File to Edit | Line Range |
|---------|--------------|------------|
| Navigation Menu | `content.json` | Lines 2-19 |
| Hero (Main Banner) | `content.json` | Lines 20-44 |
| Product Features | `pitch.html` | Lines 1483-1529 |
| Challenge Section | `pitch.html` | Lines 1532-1571 |
| Get Started Cards | `pitch.html` | Lines 1574-1610 |
| Tenant Onboarding | `pitch.html` | Lines 1612-1684 |
| App Mockups | `pitch.html` | Lines 1686-1720 |
| Trust & Security | `pitch.html` | Lines 1722-1763 |
| Contact Form (CTA) | `pitch.html` | Lines 1765-1833 |
| Footer | `pitch.html` | Lines 1836-1897 |

---

## 1. Navigation & Hero
**File:** `/Users/ronnielee/neighbr/content.json`

### Navigation Links (Lines 2-19)
```json
"navigation": {
  "features": {
    "en": "Features",        ← Change English text here
    "zh": "功能"             ← Change Chinese text here
  },
  "implementation": {
    "en": "Implementation",
    "zh": "實施流程"
  },
  // ... more navigation items
}
```

### Hero Section (Lines 20-44)
```json
"hero": {
  "badge": {
    "en": "⚡ 2-WEEK SETUP • 🎁 90 DAYS FREE • 🔒 ENTERPRISE SECURITY",
    "zh": "⚡ 兩週上線 • 🎁 免費試用90日 • 🔒 企業級網絡保安"
  },
  "title": {
    "en": "Property Management.<br><span class='highlight'>Simplified.</span>",
    "zh": "物業管理<br><span class='highlight'>化繁為簡</span>"
  },
  // ... more hero content
}
```

**How to Edit:**
1. Open `content.json` in text editor
2. Find the section (navigation or hero)
3. Edit the `"en"` value for English
4. Edit the `"zh"` value for Chinese
5. Save the file

---

## 2. Product Features
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1483-1529

### Section Header (Lines 1486-1488)

**Subtitle** (Line 1486):
```html
data-en="✨ Complete Platform"
data-zh="✨ 完整平台"
```

**Title** (Line 1487):
```html
data-en="Everything You Need in One Happy Place"
data-zh="所需的一切都在這裡"
```

**Description** (Line 1488):
```html
data-en="Replace scattered tools and endless spreadsheets with one beautiful platform your team will actually enjoy using."
data-zh="用一個美觀的平台取代零散工具和無盡的試算表,讓你的團隊真正樂於使用。"
```
👆 **This is the phrase you asked about!**

### Feature Cards (Lines 1491-1526)

Each feature card has:
- Icon (emoji)
- Title
- Description
- Benefit line

**Feature 1: Smart Maintenance Management** (Lines 1491-1496)
- Title (Line 1493): `data-en="Smart Maintenance Management" data-zh="智能維修管理"`
- Description (Line 1494): Long text about submitting issues
- Benefit (Line 1495): `data-en="Benefit: Faster resolution times..."`

**Feature 2: Automated Facility Booking** (Lines 1497-1502)
**Feature 3: Instant Announcements** (Lines 1503-1508)
**Feature 4: Centralized Communication** (Lines 1509-1514)
**Feature 5: Management Dashboard** (Lines 1515-1520)
**Feature 6: Community Features** (Lines 1521-1526)

**How to Edit:**
1. Open `pitch.html`
2. Go to the line number
3. Find `data-en="..."` and edit the English text inside the quotes
4. Find `data-zh="..."` and edit the Chinese text inside the quotes
5. Save the file

---

## 3. Challenge Section
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1532-1571

### Section Header (Lines 1535-1536)

**Subtitle** (Line 1535):
```html
data-en="😅 The Reality"
data-zh="😅 現實狀況"
```

**Title** (Line 1536):
```html
data-en="Sound Familiar? We've Got You."
data-zh="似曾相識?我們幫到你。"
```

### Your Current Challenges (Lines 1540-1553)

**Challenge 1: Simpler booking system** (Lines 1542-1544)
- Title (Line 1542): `data-en="Simpler booking system for everyone" data-zh="更簡單的預訂系統"`
- Description (Line 1543): Text about booking facilities

**Challenge 2: Tracking of maintenance** (Lines 1545-1547)
**Challenge 3: Improved safety** (Lines 1549-1552)

### How Neighbr Solves This (Lines 1555-1569)

**Solution 1: 24/7 Self-Service Booking** (Lines 1557-1559)
**Solution 2: Digital Maintenance Tracking** (Lines 1561-1563)
**Solution 3: Real-Time Safety Alerts** (Lines 1565-1568)

---

## 4. Get Started Section
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1574-1610

### Section Header (Lines 1579-1581)

**Title** (Line 1579):
```html
data-en="Get Started Risk-Free 🚀"
data-zh="零風險開始 🚀"
```

**Subtitle** (Line 1581):
```html
data-en="Everything you need to go live in 2 weeks. Then try it free for 90 days."
data-zh="兩星期內上線所需的一切。然後免費試用90日。"
```

### Cards (Lines 1584-1604)

**Card 1: Live in 2 Weeks** (Lines 1584-1587)
- Icon: ⚡
- Title (Line 1586): `data-en="Live in 2 Weeks" data-zh="兩星期內上線"`
- Description (Line 1587): Text about onboarding

**Card 2: 90 Days Free** (Lines 1589-1592)
**Card 3: Bank-Level Security** (Lines 1594-1597)
**Card 4: Local Support** (Lines 1599-1602)

**CTA Button** (Line 1606):
```html
data-en="Start Your Free 90-Day Trial →"
data-zh="開始90日免費試用 →"
```

---

## 5. Tenant Onboarding
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1612-1684

### Section Header (Lines 1616-1618)

**Subtitle** (Line 1616):
```html
data-en="📱 TENANT ACCESS"
data-zh="📱 住戶使用"
```

**Title** (Line 1617):
```html
data-en="How Tenants Join in 5 Simple Steps"
data-zh="住戶5步輕鬆登記"
```

**Description** (Line 1618):
```html
data-en="Your tenants don't need to download anything..."
data-zh="您的住戶無需下載任何程式..."
```

### Onboarding Steps (Lines 1627-1673)

Each step has:
- Icon (emoji in a circle)
- Title
- Description

**Step 1: Scan QR Code** (Lines 1627-1630)
- Icon: 📱
- Title (Line 1628): `data-en="Scan QR Code" data-zh="掃描QR碼"`
- Description (Line 1629): Instructions about posting QR codes

**Step 2: Open in Browser** (Lines 1636-1639)
**Step 3: Choose Building** (Lines 1645-1648)
**Step 4: Get Notifications** (Lines 1654-1657)
**Step 5: Start Using** (Lines 1663-1666)

---

## 6. App Mockups
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1686-1720

### Section Header (Lines 1687-1689)

**Subtitle** (Line 1687):
```html
data-en="📱 See It In Action"
data-zh="📱 實際示範"
```

**Title** (Line 1688):
```html
data-en="So Simple, Your Tenants Will Thank You"
data-zh="如此簡單,住戶會感謝你"
```

**Description** (Line 1689):
```html
data-en="Beautiful design that just works. Most tenants are actively using it within the first month..."
data-zh="美觀的設計,就是好用。首月內大部分住戶積極使用..."
```

### Mockup Descriptions (Lines 1696-1717)

**Mockup 1: Tenant Dashboard** (Lines 1696-1698)
- Title (Line 1696): `data-en="Tenant Dashboard" data-zh="住戶儀表板"`
- Description (Line 1697): About the home screen

**Mockup 2: Maintenance Reporting** (Lines 1700-1702)
**Mockup 3: Facility Booking** (Lines 1704-1706)
**Mockup 4: Announcements** (Lines 1708-1710)
**Mockup 5: Management View** (Lines 1712-1714)

---

## 7. Trust & Security
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1722-1763

### Section Header (Lines 1735-1737)

**Subtitle** (Line 1735):
```html
data-en="🔒 Enterprise-Grade Security"
data-zh="🔒 企業級保安"
```

**Title** (Line 1736):
```html
data-en="Built to Protect Your Tenants' Data"
data-zh="為保護住戶資料而設"
```

**Description** (Line 1737):
```html
data-en="Security and privacy aren't optional. They're the foundation..."
data-zh="安全和私隱並非可有可無,而是基礎..."
```

### Trust Points (Lines 1740-1760)

**Point 1: Data Privacy** (Lines 1740-1742)
- Title (Line 1740): `data-en="PDPO Compliant" data-zh="符合個人資料私隱條例"`
- Description (Line 1741): Details about compliance

**Point 2: Infrastructure** (Lines 1744-1746)
**Point 3: Uptime** (Lines 1748-1750)
**Point 4: Support** (Lines 1752-1754)

---

## 8. Contact Form (CTA Section)
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1765-1833

### Section Header (Lines 1777-1780)

**Title** (Line 1777):
```html
data-en="Ready to Make Your Life Way Easier? 🚀"
data-zh="準備好讓生活輕鬆得多?🚀"
```

**Subtitle** (Lines 1778-1780):
```html
data-en="Try Neighbr free for 90 days. Setup in 2 weeks. Then just $168/month per building. Simple as that."
data-zh="免費試用Neighbr 90日。兩星期內上線。其後每棟每月只需$168。就是這麼簡單。"
```

### Form Field Placeholders (Lines 1798-1817)

**First Name** (Line 1798):
```html
placeholder="First Name"
data-en="First Name"
data-zh="名字"
```

**Last Name** (Line 1801):
```html
data-en="Last Name"
data-zh="姓氏"
```

**Email** (Line 1807):
```html
data-en="Your work email"
data-zh="你的工作電郵"
```

**Subject** (Line 1812):
```html
data-en="Subject"
data-zh="主旨"
```

**Message** (Line 1817):
```html
data-en="Tell us about your building(s)..."
data-zh="告訴我們關於您的大廈..."
```

**Submit Button** (Line 1827):
```html
data-en="Start Free Trial →"
data-zh="開始免費試用 →"
```

---

## 9. Footer
**File:** `/Users/ronnielee/neighbr/pitch.html`
**Lines:** 1836-1897

### Footer Content (Lines 1838-1896)

**Tagline** (Line 1849):
```html
data-en="The modern property management platform built specifically for Hong Kong."
data-zh="專為香港而設的現代物業管理平台。"
```

**Mission Statement** (Line 1850):
```html
data-en="Building better communities, one building at a time."
data-zh="逐棟大廈打造更美好社區。"
```

### Footer Links

**Product Section** (Lines 1853-1857)
- Header (Line 1854): `data-en="Product" data-zh="產品"`
- Features link (Line 1855): `data-en="Features" data-zh="功能"`
- Implementation link (Line 1856): `data-en="Implementation" data-zh="實施流程"`
- Request Demo link (Line 1857): `data-en="Request Demo" data-zh="預約示範"`

**Company Section** (Lines 1859-1864)
**Contact Section** (Lines 1866-1871)

**Bottom Bar** (Lines 1874-1896)
- Copyright (Line 1881): `data-en="&copy; 2026 Neighbr. All rights reserved." data-zh="&copy; 2026 Neighbr. 版權所有。"`
- Privacy Policy (Line 1885): `data-en="Privacy Policy" data-zh="私隱政策"`
- Terms of Service (Line 1889): `data-en="Terms of Service" data-zh="服務條款"`

---

## 📝 Editing Instructions

### For content.json:
1. Open `/Users/ronnielee/neighbr/content.json`
2. Find the section you want to edit
3. Change the text inside `"en": "..."` for English
4. Change the text inside `"zh": "..."` for Chinese
5. **Important:** Keep all the `{`, `}`, `,`, `:`, and `"` characters in place
6. Save the file
7. Refresh your browser to see changes

### For pitch.html:
1. Open `/Users/ronnielee/neighbr/pitch.html`
2. Use **Cmd+F** (Mac) or **Ctrl+F** (Windows) to search for the text you want to change
3. Find the `data-en="..."` attribute
4. Edit the text **inside the quotes**
5. Find the `data-zh="..."` attribute
6. Edit the Chinese text **inside the quotes**
7. Save the file
8. Refresh your browser to see changes

---

## 🔍 Quick Find Tips

### Finding Text by Search:
1. **Copy the text** you see on the website
2. **Search** (Cmd+F / Ctrl+F) for that text in:
   - First try: `content.json`
   - If not found, try: `pitch.html`
3. Once found, you'll see it in a `data-en="..."` or `"en": "..."` attribute
4. Edit both English (`data-en` or `"en"`) and Chinese (`data-zh` or `"zh"`)

### Finding Text by Section:
1. Look at the **Table of Contents** at the top of this guide
2. Find your section
3. Note the **file name** and **line numbers**
4. Open that file and go to those lines

---

## ⚠️ Important Notes

### DO:
- ✅ Edit text inside the quotes
- ✅ Keep all HTML tags like `<br>`, `<strong>`, `<span>`
- ✅ Save the file after editing
- ✅ Test both EN and 中 language toggle after editing

### DON'T:
- ❌ Remove quotes `"` around text
- ❌ Remove commas `,` between items (in JSON)
- ❌ Delete any `{`, `}`, `[`, `]`, `:` characters (in JSON)
- ❌ Change `data-en` or `data-zh` to something else
- ❌ Remove the `=` signs

---

## 🐛 If Something Breaks

1. **Undo your changes** (Cmd+Z / Ctrl+Z)
2. **Check for:**
   - Missing quotes `"`
   - Missing commas `,` (in JSON)
   - Deleted brackets or braces
3. **For JSON files:** Validate at https://jsonlint.com
4. **Refresh browser** with hard reload (Cmd+Shift+R / Ctrl+Shift+R)

---

## 🚀 After Editing

1. **Save the file**
2. **Commit to git:**
   ```bash
   git add content.json pitch.html
   git commit -m "Update website content"
   git push origin main
   ```
3. **Check the live website** at www.neighbrhk.com (may take a few minutes to update)

---

## 📞 Need Help?

If you can't find where to edit something:
1. Copy the exact text from the website
2. Search for it in both `content.json` and `pitch.html`
3. Follow the editing instructions for whichever file contains it

**Still stuck?** Contact your technical co-founder or refer to:
- `/Users/ronnielee/neighbr/CONTENT-EDITING-GUIDE.md` (original guide)
- `/Users/ronnielee/neighbr/README-FOR-CONTENT-EDITORS.md` (quick start)

---

**Last Updated:** January 13, 2026
**Files:** content.json (lines 1-407), pitch.html (lines 1-2162)
