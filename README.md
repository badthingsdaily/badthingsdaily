# Security Tabletop Scenarios

A place for security teams to explore and discuss incident response scenarios (scenarios by Ryan McGeehan @m4goo)

## Overview

This application provides a searchable, filterable collection of security incident scenarios designed for tabletop exercises and team training. Each scenario presents a realistic security situation that teams can use to practice their incident response procedures.

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

### Building for Production

```bash
npm run build
```

This creates an optimized production build in the `build` folder.

### Deploying to GitHub Pages

1. The `homepage` field in `package.json` is already configured for:
   ```json
   "homepage": "https://badthingsdaily.github.io"
   ```
   
   Note: This requires the repository to be named `badthingsdaily.github.io` under a GitHub account/organization named `badthingsdaily`.

2. Install the gh-pages dependency (if not already installed):
   ```bash
   npm install --save-dev gh-pages
   ```

3. Deploy to GitHub Pages:
   ```bash
   npm run deploy
   ```

4. Go to your repository Settings → Pages and ensure the source is set to "Deploy from a branch" and the branch is `gh-pages`

The app will be available at the URL specified in your homepage field.

## Adding More Scenarios

Scenarios are stored in `src/scenarios.json`. To add new scenarios, edit this file and follow the format:

```json
  {
      "id": 494,
      "title": "Worst Case Scenario",
      "description": "What's the worst that can happen?"
  }
```

## Credits

These security scenarios were originally shared on [x.com/badthingsdaily](https://x.com/badthingsdaily) by [Ryan McGeehan](https://www.linkedin.com/in/m4goo/) (@badthingsdaily).

- This application is intended for educational and training purposes only
- For commercial use or redistribution of the scenarios, please contact the original author

Created with ❤️ by [Adversis](https://www.adversis.io)
