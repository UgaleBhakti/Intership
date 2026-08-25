BHAKTI UGALE PORTFOLIO - AWS S3

Files:
- index.html  -> main portfolio page
- style.css   -> website design
- script.js   -> mobile navigation
- 404.html    -> error page

LOCAL TEST:
1. Keep all files in the same folder.
2. Double-click index.html, or open it with a browser.
3. Check all navigation and contact links.

AWS S3 HOSTING:
1. Create an S3 bucket with a globally unique name.
2. Choose the AWS Region you want.
3. Upload index.html, style.css, script.js and 404.html.
4. In S3 -> Properties -> Static website hosting:
   - Enable Static website hosting
   - Hosting type: Host a static website
   - Index document: index.html
   - Error document: 404.html
5. For a public static website, configure the bucket policy/public access
   according to your AWS account's current S3 static website requirements.
6. Open the S3 website endpoint shown by AWS.

IMPORTANT:
- This portfolio contains the contact information from the supplied resume.
- If you want to add a profile photo, create an images folder and upload
  your photo, then add an <img> element to index.html.
- For production HTTPS/custom domains, use CloudFront in front of S3.
