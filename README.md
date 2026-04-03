# Antonietta Dentici - Baptism Confirmation Website

A beautiful, responsive website for collecting baptism attendance confirmations.

## Features

- **Step 1**: Guest name and baptism attendance confirmation
- **Step 2**: Reception attendance confirmation
- **Step 3**: Detailed preferences including:
  - Companion information
  - Number of guests
  - Appetizer selection (House Salad or Caesar Salad)
  - Main course selection (Roasted Chicken, Filet Mignon, Chilean Sea Bass)
  - Cocktail selection (Bourbon Old Fashioned, Berries & Bubbles) - Max 2 per person
  - Additional notes

## How to Open

Simply open `index.html` in any web browser.

## Email Configuration (Optional)

To receive confirmations via email, you need to set up EmailJS:

1. Go to [emailjs.com](https://emailjs.com) and create a free account
2. Create an Email Service (Gmail, Outlook, etc.)
3. Create an Email Template with these variables:
   - `{{guest_name}}`
   - `{{attendance}}`
   - `{{reception}}`
   - `{{companion}}`
   - `{{guest_count}}`
   - `{{appetizers}}`
   - `{{main_courses}}`
   - `{{cocktails}}`
   - `{{notes}}`
4. Copy your Public Key
5. In `index.html`, find the line:
   ```javascript
   emailjs.init('YOUR_PUBLIC_KEY');
   ```
   And replace `YOUR_PUBLIC_KEY` with your actual EmailJS Public Key.

## Preview

The website includes:
- Elegant design with soft colors
- Progress indicator
- Step-by-step form navigation
- Validation on all fields
- Thank you page with gift information
- Summary of the response

## Gift Information

The thank you page includes a message about cash gifts being welcome.

---

Made with ❤️ for Antonietta's Baptism Celebration
