# Web3Forms Setup Guide

## 🚨 IMPORTANT: Form Won't Work Until You Complete This Setup!

Your contact form needs a **Web3Forms Access Key** to send emails. Without it, submissions won't be delivered.

---

## ⚡ Quick Setup (3 Steps - Takes 5 Minutes)

### Step 1: Get Your Free Access Key

1. Open your browser and go to: **https://web3forms.com**
2. You'll see a simple form asking for your email
3. Enter: **admin@neighbrhk.com**
4. Click **"Create Access Key"** button
5. Go to your **admin@neighbrhk.com** inbox
6. Look for email from **Web3Forms** (check spam if not in inbox!)
7. Click the **verification link** in the email
8. After verification, you'll see your **Access Key** on screen
9. **COPY** the access key (it looks like: `a1b2c3d4-e5f6-7g8h-9i0j-k1l2m3n4o5p6`)

---

### Step 2: Add Access Key to Your Website

1. Open the file: **`/Users/ronnielee/neighbr/pitch.html`**
2. Search for: `YOUR_ACCESS_KEY_HERE` (around line 2063)
3. You'll find this line:
   ```html
   <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
   ```
4. Replace `YOUR_ACCESS_KEY_HERE` with your actual key:
   ```html
   <input type="hidden" name="access_key" value="a1b2c3d4-e5f6-7g8h-9i0j-k1l2m3n4o5p6">
   ```
5. **Save the file** (Cmd+S / Ctrl+S)
6. **Commit and push** to GitHub:
   ```bash
   git add pitch.html
   git commit -m "Add Web3Forms access key"
   git push origin main
   ```

---

### Step 3: Test the Form

1. Start your local server:
   ```bash
   cd /Users/ronnielee/neighbr
   python3 -m http.server 8000
   ```
2. Open: **http://localhost:8000/pitch.html**
3. Scroll to the bottom **"Ready to Make Your Life Way Easier?"** section
4. Fill out ALL form fields:
   - First Name
   - Last Name
   - Email
   - Subject
   - Message
5. Click **"Start Free Trial →"** button
6. You should see: **"✅ Thank you! We'll get back to you soon."**
7. Check **admin@neighbrhk.com** inbox within 1-2 minutes

---

## 🐛 Troubleshooting

### I'm not receiving emails!

**1. Check Spam/Junk Folder First!**
   - Web3Forms emails sometimes go to spam initially
   - Mark as "Not Spam" to train your email filter

**2. Verify Your Access Key is Correct**
   - Make sure you replaced `YOUR_ACCESS_KEY_HERE` with the actual key
   - No extra spaces before or after the key
   - Key should be inside the quotes

**3. Check Browser Console for Errors**
   - Open the website in Chrome/Firefox
   - Press F12 to open Developer Tools
   - Click "Console" tab
   - Submit the form
   - Look for any error messages (screenshot them and share if needed)

**4. Verify Email Address Used for Access Key**
   - Log into https://web3forms.com
   - Check which email address is associated with your access key
   - It MUST be **admin@neighbrhk.com**
   - If wrong, create a new access key with the correct email

### Form shows "Form configuration error"

This means the access key is invalid or missing. Double-check Step 2 above.

### Form shows "Submission failed"

This could be:
- Network issue (check your internet connection)
- Web3Forms service temporarily down (rare)
- Access key not verified yet (check email for verification link)

---

## 🔍 How to Check if Setup is Working

Open the browser console (F12 → Console tab) and submit the form. You should see:

**If working correctly:**
```
Web3Forms Response: {success: true, message: "Email sent successfully"}
```

**If access key is missing/wrong:**
```
Web3Forms Error: Access key is required
```

This will tell you exactly what the issue is!

---

## What You'll Receive

When someone submits the form, you'll get an email at **admin@neighbrhk.com** with:

- **First Name**: The user's first name
- **Last Name**: The user's last name
- **Email**: Their work email address
- **Subject**: The inquiry subject they entered
- **Message**: Their detailed message about their building(s)

---

## Free Tier Limits

Web3Forms free tier includes:
- ✅ **Unlimited submissions** per month
- ✅ No monthly limits
- ✅ No account required after initial setup
- ✅ Email notifications
- ✅ Spam protection

Much better than FormSubmit.co which required confirmation emails!

---

## Troubleshooting

### "Submission failed" error
- Make sure you've replaced `YOUR_ACCESS_KEY_HERE` with your actual key
- Verify the access key is active at web3forms.com
- Check that admin@neighbrhk.com is verified

### Not receiving emails
- Check spam/junk folder
- Verify admin@neighbrhk.com is the email you used to create the access key
- Log into web3forms.com to see submission logs

### Form fields not translating
- The form uses bilingual placeholders that change with the EN/中 toggle
- If text isn't changing, check browser console for JavaScript errors

---

## Form Fields

The contact form includes:
1. **First Name** (名字) - Required
2. **Last Name** (姓氏) - Required
3. **Email** (你的工作電郵) - Required, validated with regex
4. **Subject** (主旨) - Required
5. **Message** (告訴我們關於您的大廈) - Required, textarea with 5 rows

All fields have:
- Real-time validation
- Bilingual error messages (English/Cantonese)
- Loading state during submission
- Success confirmation message

---

## Need Help?

- Web3Forms Documentation: https://docs.web3forms.com
- Web3Forms Support: support@web3forms.com
- Alternative services if needed: Formspree, Getform, EmailJS
