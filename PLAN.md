# Plan: TikTok Content Assistant Website

## Goal

Create a small, public, static website for a private tool called **TikTok Content Assistant**.

The website must:
- Be suitable as the official Web/Desktop URL for a TikTok developer app.
- Explain what the tool does in plain language.
- Include visible, working links to Terms of Service and Privacy Policy.
- Be deployable free on GitHub Pages.
- Work well on mobile and desktop.
- Not collect data, use cookies, analytics, tracking pixels, forms, accounts, JavaScript frameworks, or external dependencies.

This is a legal-information and product-information site only. It is not a functional app, login page, OAuth callback page, or TikTok publishing UI.

## Background

TikTok Content Assistant is a private tool operated by [YOUR NAME OR BUSINESS NAME]. It lets an authorised user connect their own TikTok account through Composio to view authorised account/video information and manage, upload, or publish content at the user's direction.

TikTok should never be described as endorsing, operating, sponsoring, or being affiliated with this website or tool.

## Repository and Deployment

- Use plain static HTML and CSS only.
- No build tool, package manager, Node.js, React, server, database, or API.
- Use the repository root as the GitHub Pages publishing source.
- Files must work at: `https://[GITHUB-USERNAME].github.io/[REPOSITORY-NAME]/`
- Use relative links only, so the site works correctly under a repository path.
- Keep all content public and suitable for TikTok app review.

## Required Files

Create exactly these primary files:

- `index.html`
- `terms.html`
- `privacy.html`
- `styles.css`
- `README.md`

Optional:
- `favicon.svg`

## Design Requirements

- Clean, professional, trustworthy.
- Responsive single-column content layout, maximum readable width around 760px.
- Light background, dark readable text, one restrained accent colour.
- Use system fonts only.
- Strong colour contrast and keyboard-visible focus states.
- Semantic HTML: `header`, `nav`, `main`, `section`, `footer`.
- No fabricated customer logos, testimonials, download buttons, statistics, screenshots, social links, or claims of TikTok partnership.
- Every page must have the same header and footer.
- Navigation must include: Home, Terms, Privacy.
- Footer must show the current year as plain text, the operator name placeholder, and Terms/Privacy links.

## Homepage Content: `index.html`

### Title and metadata

- Page title: `TikTok Content Assistant`
- Meta description: `A private tool for authorised TikTok account connection and content management.`

### Visible content

Use this exact structure and substantially this wording:

1. Hero
   - H1: `TikTok Content Assistant`
   - Short description: `A private tool for connecting an authorised TikTok account to manage content through Composio.`

2. What the tool does
   - Explain: `The tool helps an authorised user connect their own TikTok account, view information they have permitted access to, and manage, upload, or publish content at their direction.`

3. Account and permission notice
   - Explain: `Only connect a TikTok account that you own or are authorised to manage. Permissions are requested through TikTok's authorisation process and can be revoked at any time through TikTok or the connected-service settings.`

4. Data handling summary
   - Explain: `The tool uses TikTok and Composio to provide the requested connection. It does not request or store a TikTok password. Read the Privacy Policy for details about information handling.`

5. Contact
   - Show: `Contact: [YOUR CONTACT EMAIL]`
   - Make the email a mailto link.

6. Footer
   - Include clear links to `terms.html` and `privacy.html`.

## Terms Content: `terms.html`

Use an H1 of `Terms of Service`.

Include this text, replacing only placeholders in square brackets:

Last updated: [DATE]

TikTok Content Assistant ("the Service") is a private content-management tool operated by [YOUR NAME OR BUSINESS NAME] ("we", "us").

### 1. Service
The Service lets authorised users connect their TikTok account through Composio to manage, upload, and publish content where the user has granted permission.

### 2. Eligibility and account access
You must be legally permitted to use TikTok and must connect only TikTok accounts that you own or are authorised to manage. You are responsible for protecting your accounts and for activity carried out through the Service.

### 3. Your content
You retain ownership of content you provide. You confirm that you have all rights needed to upload or publish that content and that it complies with TikTok's terms, community guidelines, and applicable law.

### 4. Third-party services
The Service uses TikTok and Composio. Their services are governed by their own terms and policies. We do not control their availability, rules, or actions.

### 5. No guarantee
The Service is provided "as is" and "as available." We do not guarantee that uploads, publishing, or third-party integrations will always work without interruption or error.

### 6. Suspension or termination
We may suspend or end access where necessary for security, legal compliance, or misuse. You may stop using the Service at any time and revoke TikTok access through your TikTok settings.

### 7. Changes
We may update these Terms. Continued use after an update means you accept the updated Terms.

### 8. Contact
Questions: [YOUR CONTACT EMAIL]  
Operator: [YOUR NAME OR BUSINESS NAME]  
Location: United Kingdom

## Privacy Content: `privacy.html`

Use an H1 of `Privacy Policy`.

Include this text, replacing only placeholders in square brackets:

Last updated: [DATE]

[YOUR NAME OR BUSINESS NAME] operates TikTok Content Assistant ("the Service").

### 1. Information we process
When you connect TikTok, we may process the information and permissions you authorise, such as TikTok profile information, account statistics, video information, and content you choose to upload or publish.

### 2. Why we use it
We use this information only to provide the features you request: connecting your TikTok account, displaying authorised information, and managing, uploading, or publishing content at your direction.

### 3. OAuth tokens
TikTok access tokens are managed through Composio to maintain the authorised connection. We do not ask for or store your TikTok password.

### 4. Sharing
We share data only with service providers needed to operate the Service, including Composio and TikTok, or where required by law. We do not sell personal information or use TikTok data for advertising.

### 5. Retention
We keep data only for as long as necessary to provide the Service, meet legal obligations, resolve disputes, and maintain security. You can revoke TikTok access at any time; this stops future authorised access.

### 6. Security
We use reasonable technical and organisational measures to protect information. No online system can be guaranteed completely secure.

### 7. Your choices
You may ask to access, correct, or delete personal information we hold by contacting us. You may revoke TikTok access through TikTok settings or the Service connection settings.

### 8. International processing
Your information may be processed in countries where TikTok, Composio, or their service providers operate.

### 9. Changes
We may update this policy and will publish the updated version with a new "Last updated" date.

### 10. Contact
Privacy questions or deletion requests: [YOUR CONTACT EMAIL]  
Operator: [YOUR NAME OR BUSINESS NAME]  
Location: United Kingdom

## README Requirements

Write concise setup instructions:

1. Replace every placeholder:
   - `[YOUR NAME OR BUSINESS NAME]`
   - `[YOUR CONTACT EMAIL]`
   - `[DATE]`
2. Create a public GitHub repository.
3. Upload or commit these files to the `main` branch.
4. In GitHub: Settings → Pages → Build and deployment:
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/ (root)`
5. Wait for the GitHub Pages URL to become available.
6. Verify all three URLs load publicly:
   - `/`
   - `/terms.html`
   - `/privacy.html`
7. Enter those URLs into the corresponding TikTok app fields.

Include a reminder:
- Do not put the Composio OAuth callback URL in the Web/Desktop URL field.
- Enter the Composio callback only in TikTok Login Kit's Redirect URI setting: `https://backend.composio.dev/api/v1/auth-apps/add`

## Acceptance Criteria

- Site has no broken relative links when hosted at a GitHub Pages repository URL.
- Home, Terms, and Privacy all load without JavaScript.
- Terms and Privacy links are visible in both header and footer on every page.
- Website describes the tool and is not merely a blank landing page.
- There are no untrue claims about affiliation with TikTok or Composio.
- All placeholders are clearly marked for manual replacement.
- HTML passes basic semantic and accessibility checks.
- GitHub Pages can deploy it without a build step.
