# Quick Start: Editing Neighbr Website Content

## 📝 What You Need to Know

You can now edit the website content **without touching any HTML code**!

## 🎯 THE FILE YOU'LL EDIT

```
/Users/ronnielee/neighbr/content.json
```

**This is your single file for editing website text in English and Cantonese.**

---

## 🚀 Quick Start (3 Steps)

### Step 1: Open the file
Open `content.json` in any text editor:
- **VS Code** (recommended)
- **Sublime Text**
- **TextEdit** (works but not ideal)

### Step 2: Edit the content
Find the section you want to change and edit the text:

```json
{
  "hero": {
    "title": {
      "en": "Your English Text Here",
      "zh": "你的中文內容"
    }
  }
}
```

- **For English:** Edit the `"en"` value
- **For Cantonese:** Edit the `"zh"` value

### Step 3: Save and preview
1. Save the file
2. Start the local server:
   ```bash
   cd /Users/ronnielee/neighbr
   python3 -m http.server 8000
   ```
3. Open browser: http://localhost:8000/pitch.html
4. Click EN/中 to toggle languages

---

## 📚 Full Documentation

For detailed instructions, examples, and tips:
```
/Users/ronnielee/neighbr/CONTENT-EDITING-GUIDE.md
```

---

## ✅ Currently Editable via JSON

These sections load from `content.json`:
- Navigation menu (top bar and mobile menu)
- Hero section (main banner with title and buttons)

**All other sections** currently need to be edited in `pitch.html` using the `data-en` and `data-zh` attributes (we can migrate more sections to JSON as needed).

---

## ⚠️ Important Rules

### DO:
- ✅ Edit text inside the quotes
- ✅ Keep all the `{`, `}`, `[`, `]`, `:`, `,` in place
- ✅ Use `<br>` for line breaks
- ✅ Use `<strong>` for bold text
- ✅ Save after every change

### DON'T:
- ❌ Remove quotes around text
- ❌ Remove commas between items
- ❌ Delete any curly braces or brackets
- ❌ Use fancy quotes (use straight quotes: `"`)

---

## 🆘 If Something Breaks

1. **Undo your last change** (Cmd+Z / Ctrl+Z)
2. **Check for missing commas or quotes**
3. **Validate your JSON:** Copy the file content and paste into https://jsonlint.com/
4. **Ask for help!**

---

## 📍 File Locations Quick Reference

| What | Where |
|------|-------|
| **Edit content here** | `/Users/ronnielee/neighbr/content.json` |
| **Full guide** | `/Users/ronnielee/neighbr/CONTENT-EDITING-GUIDE.md` |
| **Website file** | `/Users/ronnielee/neighbr/pitch.html` |

---

## 🎓 Example Edit

**Want to change the hero title?**

**Before:**
```json
{
  "hero": {
    "title": {
      "en": "Property Management.<br><span class='highlight'>Reimagined.</span>",
      "zh": "物業管理。<br><span class='highlight'>重新定義。</span>"
    }
  }
}
```

**After:**
```json
{
  "hero": {
    "title": {
      "en": "Property Management.<br><span class='highlight'>Simplified.</span>",
      "zh": "物業管理。<br><span class='highlight'>化繁為簡。</span>"
    }
  }
}
```

Save → Refresh browser → Done! ✨

---

**Need help? Just ask!**
