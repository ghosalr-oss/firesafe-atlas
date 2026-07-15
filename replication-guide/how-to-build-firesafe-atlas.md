# How To Build FireSafe Atlas For Another Rural Community

This replication guide explains how another student, school, NGO, or community group can reuse the FireSafe Atlas method.

## Version 1 Hosting Model

Use a static public dashboard, not a VM.

Recommended default:

```text
GitHub Pages
```

The dashboard should use static files:

```text
dashboard/index.html
dashboard/styles.css
dashboard/app.js
dashboard/data/*.geojson
```

This makes the project free to host, easy to copy, and suitable for communities that do not have cloud infrastructure.

## When A VM Might Be Needed

A VM should only be considered if a future version needs live user uploads, logins, a database, scheduled data jobs, or server-side GIS processing.

For version 1, the intern should document why GitHub Pages is enough and publish the working public dashboard URL.
