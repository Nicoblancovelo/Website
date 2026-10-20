SIMPLE PHOTO GALLERY FOR NETLIFY + PAGES CMS
===========================================

CONTENTS
  gallery.html          Public gallery page
  gallery.json          Photograph list and captions
  .pages.yml            Pages CMS configuration
  images/               Uploaded photos live here

ADD TO AN EXISTING NETLIFY WEBSITE

1. Edit gallery.html: replace the two instances of "Your Name" with your name.

2. Put gallery.html, gallery.json, .pages.yml and images/ in the ROOT
   of the same folder/repository as your website's index.html.
   Do not put them in a second nested subfolder.
   The .pages.yml file is hidden by default on some operating systems.

3. Your website should be stored in a GitHub repository. If you previously
   deployed to Netlify by dragging and dropping files, upload your existing
   website files and these gallery files to a GitHub repository, then connect
   that repository to Netlify as your production deploy source.
   Netlify's existing site can normally be linked to a repository from its
   build/deployment configuration. Check the current Netlify UI.

4. Go to https://app.pagescms.org and sign in with GitHub. Authorize Pages
   CMS to access the repository, then open its "Photo gallery" editor.

5. Add a new "Photographs" item. Upload/select a photograph and write its
   caption. Save/publish the change. Pages CMS saves these changes to GitHub;
   Netlify redeploys automatically, with no manual folder upload.

6. Your gallery appears at https://YOURDOMAIN/gallery.html
   Link to that page from your existing homepage if desired.

IMPORTANT
  - This is plain static HTML, CSS and JavaScript: no build tool necessary.
  - The gallery starts empty; upload photos through Pages CMS.
  - Images are stored in your GitHub repository, not on Imgur.
  - Resize/compress photos before upload to avoid unnecessarily large files.
  - It assumes your website is published from the repository root.
    If Netlify has a separate publish directory, put gallery.html, gallery.json
    and the images directory inside that published directory and adjust the
    Pages CMS media path / gallery.json path as necessary.
  - If you add many full-resolution images, use a dedicated photo storage
    solution rather than committing originals to GitHub.
