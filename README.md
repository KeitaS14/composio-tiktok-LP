# TikTok Content Assistant

A small, public, static website for a private tool called **TikTok Content Assistant**.
Its purpose is to provide the official **Web/Desktop URL** required for a TikTok
developer app, so that a TikTok account can be connected through **Composio**.

This is a legal-information and product-information site only. It is **not** a
functional app, login page, OAuth callback page, or TikTok publishing UI. It uses
no JavaScript, no frameworks, no build tools, and no external dependencies.

## Files

| File             | Purpose                                            |
| ---------------- | -------------------------------------------------- |
| `index.html`     | Homepage: what the tool does, notices, contact     |
| `terms.html`     | Terms of Service                                    |
| `privacy.html`   | Privacy Policy                                      |
| `styles.css`     | All styling (responsive, system fonts, one accent) |
| `favicon.svg`    | Simple favicon (optional)                           |

## How to deploy on GitHub Pages

> All placeholders (`[YOUR NAME OR BUSINESS NAME]`, `[YOUR CONTACT EMAIL]`,
> `[DATE]`) have already been replaced in this repository with:
> - Operator name: **Keita Saito**
> - Contact email: **kaismithbook@outlook.com**
> - Date: **August 4, 2026**
>
> Update the date only when you change the Terms or Privacy text.

1. Create a **public** GitHub repository.
2. Upload (or commit) these files to the `main` branch in the repository root.
3. In GitHub: **Settings → Pages → Build and deployment**
   - **Source:** Deploy from a branch
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Wait a minute or two for the GitHub Pages URL to become available. It will look
   like:
   `https://<github-username>.github.io/<repository-name>/`
5. Verify all three URLs load publicly:
   - `https://<github-username>.github.io/<repository-name>/`
   - `https://<github-username>.github.io/<repository-name>/terms.html`
   - `https://<github-username>.github.io/<repository-name>/privacy.html`
6. Enter those URLs into the corresponding **TikTok app fields**:
   - **Web/Desktop URL** → the homepage URL above
   - **Terms of Service URL** → the `terms.html` URL above
   - **Privacy Policy URL** → the `privacy.html` URL above

## ⚠️ Important: do not confuse the Composio callback URL

- Do **not** put the Composio OAuth callback URL in the **Web/Desktop URL** field.
- The Composio callback goes **only** in TikTok Login Kit's **Redirect URI** setting:

  ```
  https://backend.composio.dev/api/v1/auth-apps/add
  ```

## Notes

- The site uses **relative links only**, so it works correctly under a repository
  subpath (e.g. `username.github.io/repository-name/`).
- All three pages load fully with **JavaScript disabled**.
- No analytics, cookies, tracking pixels, forms, or external requests are used.
