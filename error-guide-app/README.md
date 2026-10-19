# Error Code Guide Builder

A one-page web app for filling out an error code guide (Error Code / Possible Problem / Steps to Fix)
and downloading it as a formatted Excel file.

- **Download Excel** – saves the guide in the same layout as `Error Code Guide - Blank.xlsx`.
- **Open Excel** – loads a guide you made earlier (or the blank template) so you can edit it.
- **Saving progress** – everything you type saves automatically in your browser, so you can close the
  app and continue another day. A green "Saved" badge shows the last save time.
- **My guides** – keep several guides in progress (e.g. one per machine) and switch between them.
- **Cloud save (other computers)** – click **☁ Cloud save** to keep guides in a *private* GitHub repo
  (`guide-saves`) and open them on any computer. Setup, once per computer:
  1. First time only: create a private repo named `guide-saves`.
  2. Create a fine-grained token at GitHub → Settings → Developer settings → Fine-grained tokens:
     *Only select repositories → guide-saves*, *Contents: Read and write*.
  3. Paste the token in the app and click **Connect**.
  Changes upload a few seconds after you stop typing. If the same guide is edited on two computers,
  the most recent edit wins.
- Without cloud save, you can still move work with **Download Excel** and **Open Excel**.
  Private/incognito windows don't keep saved work.

Hosted with GitHub Pages by `.github/workflows/pages.yml`. To turn it on once:
repo **Settings → Pages → Build and deployment → Source: GitHub Actions**, then re-run the
"Deploy error guide app" workflow from the **Actions** tab.
