# GitHub Pages Deployment

This task makes FireSafe Atlas publicly available without running a paid server or VM.

## Assigned To

**Neil Panchal**  
Role: Intern / Research & GIS Support

## Account Setup

Neil Panchal should create a GitHub account using his Seaside email credentials.

Recommended GitHub username:

```text
neil-panchal-seaside
```

If that username is unavailable, use the closest professional variation and send the exact username to Rhea Ghosal.

Rhea Ghosal should then add Neil Panchal as a collaborator:

1. Open `https://github.com/ghosalr-oss/firesafe-atlas`.
2. Go to `Settings`.
3. Open `Collaborators and teams`.
4. Click `Add people`.
5. Search for Neil Panchal's GitHub username.
6. Grant **Write** access.
7. Do not grant Admin access.

Neil Panchal should never use Rhea Ghosal's GitHub token, password, or personal credentials.

## Deployment Task

Neil Panchal should publish the static dashboard through GitHub Pages.

1. Confirm these files exist:

   ```text
   dashboard/index.html
   dashboard/styles.css
   dashboard/app.js
   dashboard/data/sample-vulnerability-map.geojson
   dashboard/data/sample-community-assets.geojson
   ```

2. In the repository, open `Settings`.
3. Click `Pages`.
4. Set source to `Deploy from a branch`.
5. Set branch to `main`.
6. Set folder to `/root`.
7. Save the settings.
8. Wait for GitHub Pages to publish the site.
9. Test the dashboard URL:

   ```text
   https://ghosalr-oss.github.io/firesafe-atlas/dashboard/
   ```

10. Take a screenshot showing that the dashboard loads.
11. Record the public URL in the final report and README.

## VM Decision Rule

The project should not use a VM for the first version.

Use GitHub Pages unless the project later needs:

- user logins,
- file uploads,
- a live database,
- server-side GIS processing,
- scheduled data refresh jobs, or
- private API keys that cannot be exposed in browser JavaScript.

If any of those are needed later, Neil Panchal should write a one-page VM justification comparing GitHub Pages, Cloudflare Pages, Oracle Cloud Always Free, and Google Cloud Free Tier before any VM is created.

## Deliverables

By the end of the deployment task, Neil Panchal must submit:

- confirmed GitHub username,
- screenshot of collaborator access,
- screenshot of the GitHub Pages settings,
- working public dashboard URL,
- one-paragraph explanation of why a VM is not needed for version 1,
- list of any dashboard limitations.
