# Hasitha Muthumal | Portfolio

Exported from published version 17, commit a0d35ea7af8b33967fd76af07f43f6464b82f2d7.

The complete static site is in dist/. The HTML, CSS, JavaScript and SVG are in
dist/index.html. Images, credential files, and the display font and its license
are included. No dependency installation or compilation is needed.

## AWS Amplify Hosting

Git deployment: extract the archive and commit the extracted files at the
repository root. Connect the repo to Amplify Hosting. The included amplify.yml
uses test -f dist/index.html as a verification-only build command and dist as
the artifact directory.

Manual deployment: extract this archive, then ZIP the contents of dist/ with
index.html at the root of the upload ZIP. From the extracted project root:

    (cd dist && zip -r ../amplify-upload.zip .)

Upload amplify-upload.zip via Deploy without Git.

The site is browser-only. ChatGPT Sites supplied the hostname, deployment
configuration, and owner-only access. Amplify replaces those hosting services.
Set access controls before deployment if you want the site to remain private.
The credential images and PDF are served as static files alongside the site.
Project demos and social links continue to point to their existing destinations.
