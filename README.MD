CIPHER::AUDIT — Schema & Search Visibility Console
CIPHER::AUDIT is a lightweight, zero-dependency, single-file web console designed to validate structured data (Schema.org), analyze Google Search Console performance metrics, and deliver targeted AI recommendations for SEO and Google AI Overview eligibility.

Key Features
Schema Validation Engine: Parses  blocks and raw JSON-LD graphs. Validates required and recommended properties for core types (Person, Organization, Article, JobPosting, WebSite, BreadcrumbList, and more).

Search Visibility Diagnostics: Parses raw Google Search Console CSV exports. Calculates weighted positioning, blended CTR, impression distributions, and flags underperforming CTR targets.

Context-Aware AI Co-Pilot: Direct browser integration with Anthropic's Claude 3.5 Sonnet API to generate plain-language repair guides and growth strategies.

Local Artifact Storage: Built-in persistence engine using browser LocalStorage to save, view, and reload historical audit sessions without external databases.

Zero Infrastructure Requirements: Runs entirely client-side. No Node.js runtime, build steps, or server-side frameworks required.

Getting Started
Quick Start (Local)
Clone or download this repository:
git clone https://github.com/lord-saviord1/cipher-audit.git
cd cipher-audit

Open index.html in any web browser.

Usage Walkthrough
1. Schema Audit
Copy the full source code (or JSON-LD block) of any website page.

Navigate to the Schema Audit tab.

Paste the markup and click Run Audit.

View real-time error flags, compliance scores, and click Get AI Recommendations for actionable optimization steps.

2. Search Performance Analysis
Open Google Search Console.

Go to Performance -> Export -> Download CSV (Queries.csv or Pages.csv).

Drag and drop the CSV into the Search Visibility tab or paste the raw CSV content.

Click Analyze Data to view key performance indicators and high-potential opportunity keywords.

3. AI Co-Pilot Integration
Go to Settings & Artifacts.

Save your Anthropic API Key.

Use the AI Assistant tab or prompt buttons across the application to get contextual strategy advice based on your current session data.

One-Click Deployment
Deploying to GitHub Pages
Push this repository to GitHub.

Go to Settings -> Pages.

Under Branch, select main and root /.

Click Save. Your console will be live at https://lord-saviord1.github.io/cipher-audit/.

Deploying to Vercel / Netlify
Simply drag and drop the folder containing index.html into your Vercel or Netlify dashboard. Because it's a single static file, zero configuration is required.

Privacy & Security
Client-Side Only: No data uploaded to this tool ever leaves your browser unless an API call is explicitly made to Anthropic.

Key Storage: API Keys are saved strictly inside your browser's localStorage (cipher_anthropic_key). They are never transmitted to intermediate proxy servers or third-party tracking services.

License
Distributed under the MIT License. See LICENSE for details.