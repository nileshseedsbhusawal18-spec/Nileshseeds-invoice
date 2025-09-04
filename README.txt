निलेश सीड्स Invoice Website
---------------------------------
Files:
- index.html  -> Main invoice app (single file, embedded images)
- settings.html -> Configure Google Sheets (open in new tab from app)
- sample_template.csv -> Headers for your Sheet (use on 'Sheet1')
Hosting:
- Netlify: https://app.netlify.com/drop  (drag-drop both HTML files)
- GitHub Pages: create repo, upload both HTML files, enable Pages

Google Sheets:
1) Create Google Cloud project -> enable "Google Sheets API".
2) Create Service Account -> download JSON key.
3) Share your Google Sheet with service account email as Editor.
4) Open settings.html and paste Sheet ID + JSON.
5) Back on index.html, press Save on an invoice -> auto appends rows.

Notes:
- Browser CORS/security may affect service account JWT token request in some environments. If sync fails, CSV/JSON exports still work.
- Encrypted JSON backups use password @Jain2202 (change in settings if you wish).
