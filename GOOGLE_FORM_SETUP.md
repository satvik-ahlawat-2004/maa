# Google Form Setup Instructions for AYUVOYAGE Website

## Step-by-Step Guide

### 1. Create Your Google Form

1. Go to [Google Forms](https://forms.google.com)
2. Click **"Blank"** to create a new form
3. Name your form: "AYUVOYAGE - Contact Form" or similar

### 2. Add Form Fields

Add the following fields in order:

1. **Full Name**
   - Type: Short answer
   - Required: ✓

2. **Country of Residence**
   - Type: Short answer
   - Required: ✓

3. **Email**
   - Type: Short answer
   - Required: ✓
   - Validation: Email format

4. **WhatsApp / Phone Number**
   - Type: Short answer
   - Required: ✓

5. **I am:**
   - Type: Multiple choice
   - Options:
     - A wellness seeker
     - A hospital/retreat
   - Required: ✓

6. **Preferred Focus:**
   - Type: Multiple choice
   - Options:
     - Stress Management
     - Detox
     - Mental Health Therapy
     - Chronic Pain
     - General Wellness
     - Other
   - Required: ✓

7. **Approximate Budget**
   - Type: Multiple choice
   - Options:
     - Under $5,000
     - $5,000 - $10,000
     - $10,000 - $20,000
     - $20,000 - $50,000
     - Over $50,000
   - Required: ✓

8. **Tentative Travel Dates**
   - Type: Short answer
   - Required: ✓
   - Placeholder: "e.g., Q2 2025, June 2025"

9. **Message / Special Requirements**
   - Type: Paragraph
   - Required: ✗ (Optional)

### 3. Get the Embed Code

1. Click the **"Send"** button (top right of the form)
2. Click the **"</>"** (embed HTML) icon
3. Adjust the width and height if needed (recommended: width 100%, height 1400px)
4. Copy the entire iframe code

### 4. Add to Your Website

1. Open `index.html` in a text editor
2. Find the section that says `<!-- REPLACE THIS IFRAME WITH YOUR GOOGLE FORM EMBED CODE -->`
3. Replace the placeholder iframe with your copied Google Form embed code
4. Save the file

### 5. Link to Google Sheets (Automatic)

- Google Forms automatically creates a Google Sheet for responses
- To view responses:
  1. Open your Google Form
  2. Click the **"Responses"** tab
  3. Click the **Google Sheets icon** (green spreadsheet icon) to open/view responses

### 6. Adjust Form Height (Optional)

If your form is longer or shorter, adjust the CSS:

1. In `index.html`, find `.google-form-wrapper` in the `<style>` section
2. Change the `padding-bottom` value to match your form's height
   - Example: If your form is 1600px tall, set `padding-bottom: 1600px;`

## Example Embed Code Format

```html
<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfYOUR_FORM_ID_HERE/viewform?embedded=true" 
        width="100%" 
        height="1400" 
        frameborder="0" 
        marginheight="0" 
        marginwidth="0">Loading…</iframe>
```

## Notes

- All form submissions will automatically be saved to a Google Sheet
- You can access the responses in real-time
- The form is fully responsive and will work on mobile devices
- No backend code needed - Google Forms handles everything!

