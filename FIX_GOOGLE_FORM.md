# Fix: "This document is not published" Error

## Quick Fix Steps:

### Step 1: Open Your Google Form
Go to: https://docs.google.com/forms/d/1uJ6BCkO_UTy4NB3n1GIhg6jbBGR6GHDQ-wFj1U-CnpA/edit

### Step 2: Publish the Form
1. Click the **"Send"** button (top right corner)
2. You'll see sharing options

### Step 3: Get the Embed Code
1. In the "Send" popup, click the **`</>`** icon (Embed HTML) at the top
2. You'll see the embed code with an iframe
3. **Copy the entire iframe code** - it will look like:
   ```html
   <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfXXXXXXXXX/viewform?embedded=true" width="640" height="1400" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
   ```

### Step 4: Update Your Website
1. Open `index.html` in a text editor
2. Find line ~1433 (the iframe tag)
3. Replace the ENTIRE iframe tag with the code you copied from Google Forms
4. Save the file
5. Refresh your browser

### Important Notes:
- The embed code from Google Forms will have a different URL format (starts with `/d/e/1FAIpQLS...`)
- Make sure to copy the COMPLETE iframe code, not just the URL
- The form must be accessible to "Anyone with the link" for embedding to work

### Alternative: If you want to share the form link instead
If embedding doesn't work, you can also add a button that links directly to the form:
- Form link: https://docs.google.com/forms/d/1uJ6BCkO_UTy4NB3n1GIhg6jbBGR6GHDQ-wFj1U-CnpA/viewform

