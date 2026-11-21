# Sabri Mazahim — Business Analyst Portfolio

This repository hosts the portfolio site at **https://sabrizeek.github.io/**.

## Publish the supplied portfolio ZIP

1. Upload the **original ZIP file** `BA_Portfolio_Website_Publish(1).zip` to the **root of the `main` branch** using [GitHub's upload page](https://github.com/Sabrizeek/Sabrizeek.github.io/upload/main). Commit the upload. You do **not** need to unzip the archive.
2. In [Settings → Pages](https://github.com/Sabrizeek/Sabrizeek.github.io/settings/pages), set **Build and deployment → Source** to **GitHub Actions**.
3. The workflow `.github/workflows/deploy-portfolio.yml` extracts the ZIP and publishes the site. Check the [Actions tab](https://github.com/Sabrizeek/Sabrizeek.github.io/actions) for the workflow result.
4. Open https://sabrizeek.github.io/ and test the CV, case-study PDFs, and project pages.

The upload is required because ChatGPT's GitHub connector can create text files but cannot directly transfer the chat's binary ZIP/PDF/image attachments into this repository.

### Package contents

The supplied ZIP includes the main HTML page, eight project pages, styling and scripting, workflow diagrams, three PDF documents, and editable Business Analysis documents.
