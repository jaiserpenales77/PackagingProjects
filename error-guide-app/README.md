# Project Hub

A web app for packaging projects. Its **Troubleshoot Guides** tab fills out an error code guide (Error Code / Possible Problem / Steps to Fix)
and downloads it as a formatted Excel file.

- **Download Excel** – saves the guide in the same layout as `Error Code Guide - Blank.xlsx`.
- **Open Excel** – loads a guide you made earlier (or the blank template) so you can edit it.
- **Saving progress** – everything you type saves automatically in your browser, so you can close the
  app and continue another day. A green "Saved" badge shows the last save time.
- **My guides** – keep several guides in progress (e.g. one per machine) and switch between them.
- **Pictures** – each error code can have a picture (from a file or a phone camera). Click a picture to mark the
  problem area with a box, circle, arrow or label; the rest of the photo can be dimmed. A machine picture goes on its own
  "Machine Map" tab in the Excel file. Pictures are included in the Excel download and come back with Open Excel.
  Photos are not published with the app: they stay in your browser and, with cloud save, in locked files.
- **Cloud save with a password (other computers)** – click **☁ Cloud save**.
  - *First computer, once:* click the link to create a GitHub key (only the "gist" box is ticked),
    paste it, and choose an app password.
  - *Every other computer:* click **☁ Cloud save** and type the password.
  Guides and the key are encrypted with the password in the browser (AES-256-GCM, PBKDF2 600k) and
  stored in one gist (`error-guide-saves.json`) on your GitHub account; without the password the
  gist is unreadable. Changes upload a few seconds after you stop typing; if the same guide is edited
  on two computers, the most recent edit wins. When the key expires, sign out and set up again with a
  new key and the same password. Pictures are kept as separate locked files in a second gist and are only
  uploaded once.
- Without cloud save, you can still move work with **Download Excel** and **Open Excel**.
  Private/incognito windows don't keep saved work.

Hosted with GitHub Pages by `.github/workflows/pages.yml`. To turn it on once:
repo **Settings → Pages → Build and deployment → Source: GitHub Actions**, then re-run the
"Deploy Project Hub" workflow from the **Actions** tab.
