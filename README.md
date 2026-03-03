<div align="center">
  <h1>JS Recon - Bug Hunter Edition</h1>
  <p><strong>A powerful, client-side only JavaScript enumerator and beautifier custom-built for bug bounty hunters and penetration testers.</strong></p>
  
  <a href="https://chinnuy.gitlab.io/js-recon/">
    <img src="https://img.shields.io/badge/Live_Demo-Access_Now-fc6d26?style=for-the-badge&logo=gitlab" alt="Live Demo">
  </a>
</div>

<br>

JS Recon allows you to instantly fetch, perfectly beautify, and aggressively parse any minified JavaScript file to extract **over 40+ bug bounty hunting categories** directly in your browser. Since it operates entirely client-side, your targets and code are never logged to an external backend server.

---

## Features
- **Instant Beautification**: Uses optimized `js-beautify` configurations to instantly expand compressed code into highly readable, line-by-line developer formatting without breaking strings or logic.
- **Bulk URL Analysis**: Paste a list of multiple target URLs to analyze them all in a single consolidated report.
- **Domain Recon**: Provide a root domain to automatically discover and analyze all JS files referenced on its homepage.
- **Cross-Origin Fetching**: Bypasses restrictive CORS policies to pull target `.js` files using proxy routing.
- **Deep Extraction Engine**: Accurately parses minified/obfuscated code to discover:
  - **Domains & IPs**: Base hostnames, internal IPv4 subnets, localhost references.
  - **Attack Surface**: Full URLs, API Endpoints, versioned routes (`/v1/`, `/v2/`), GraphQL definitions, Webhooks, Websockets.
  - **Secrets & Keys**: Automatically flags API Keys, JWTs, Bearer tokens, AWS `AKIA` keys, and raw Private Keys.
  - **Cloud Infra**: S3 buckets, Firebase databases, CloudFront CDNs.
  - **Parameters & Roles**: Hidden `?debug=` and `?admin=` logic, local `isAdmin=true` assignments.
- **Interactive UI**: Click any extracted item in the dynamic sidebar to instantly scroll to and highlight its exact declaration in the main code editor.
- **Vibrant Theming**: Built with a sleek, premium dark-mode GitHub style layout and categorized, color-coded extraction tables.

## Live Demo
Access the fully hosted static application here:
👉 **[https://chinnuy935.github.io/js-recon/](https://chinnuy935.github.io/js-recon/)**

## Usage
1. Open the Live Demo.
2. **Fetch URL**: Paste a link to any target `.js` file (e.g. `https://target.com/assets/main.min.js`) and click "Fetch URL". 
3. **Upload Local**: Alternatively, choose a local file from your system.
4. Click **Beautify Code** to format the script. Wait a second, and the Extracted Data sidebar will automatically populate with everything it found.
5. Click on an extracted endpoint, string, or key to highlight it in the code view.

## Local Installation
Because this is a completely static tool with zero backend dependencies, you can run it locally in seconds:

1. Clone the repository:
   ```bash
   git clone https://github.com/chinnuy935/js-recon.git
   ```
2. Open `index.html` directly in any modern web browser.
   *(No `npm install`, Node.js, or Docker required!)*

---
  <i>Designed by chinnuy935</i>
</div>
