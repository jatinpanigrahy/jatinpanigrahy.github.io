# Portfolio Website

A fast, interactive personal portfolio website. Built with Astro, featuring automated build-time data fetching and a clean, responsive design.

**🔗 [View Live Application](https://jatinpanigrahy.github.io/)**

## Core Features

- **Dynamic Data:** Instantly view pinned and featured repositories pulled directly from GitHub.
- **Language Analytics:** Displays the top programming languages used in each project.
- **Zero-JS Frontend:** Achieves maximum performance by omitting client-side JavaScript entirely.

## Technical Overview

The application interfaces directly with the GitHub GraphQL API during the build process. This build-time fetching ensures that no API tokens are exposed and no client-side requests are needed. It is backed by a continuous integration pipeline (GitHub Actions) for automated nightly rebuilds to keep the data synchronized.

## UI & Design

- **Clean, Focused Design:** A custom CSS theme provides a distraction-free, highly readable interface.
- **Fast Loading:** The application relies on system fonts and CSS-only interactions to minimize loading times and reduce external dependencies.

## Tech Stack

- **Language:** TypeScript, HTML, CSS
- **Framework:** Astro
- **API:** GitHub GraphQL API
- **CI/CD:** GitHub Actions

## Running it Locally

1. Ensure you have Node.js (v20 or higher) installed on your system.

2. Clone the repository:

   ```bash
   git clone https://github.com/jatinpanigrahy/jatinpanigrahy.github.io.git
   cd jatinpanigrahy.github.io
   ```

3. Install the required dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the root directory and add your GitHub Personal Access Token (so it can fetch your pinned repos):

   ```
   GITHUB_TOKEN=your_personal_access_token
   ```

5. Launch the local development server:

   ```bash
   npm run dev
   ```

## Deployment

This application is deployed and hosted via GitHub Pages, with a nightly GitHub Actions cron job automating the build process.

**Live Application:** <https://jatinpanigrahy.github.io/>
