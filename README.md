# ICAIDIET'26 — MEC Conference Hub

Conference website for the International Conference on AI-Driven Innovation in Engineering & Technology, hosted by Muthayammal Engineering College.

## Development

Requires Node.js 22 or later.

```sh
npm ci
npm run dev
```

Create a local `.env` from `.env.example` to configure email delivery. Do not commit `.env` or secret values.

## Deployment

This is a TanStack Start application with server-side `/api/register` and `/api/contact` endpoints. GitHub Pages only serves static files, so selecting the repository root as a Pages source shows this README and cannot run the site's API endpoints.

Deploy the full application on Render:

1. In Render, choose **New** → **Blueprint**.
2. Connect the `MohanRajS-01/mec` GitHub repository and select `main`.
3. Render reads `render.yaml` and creates the Node web service.
4. Add any email provider secrets in the Render service's environment settings. Keep them out of GitHub.

The generated `onrender.com` URL is the live website. Future pushes to `main` trigger redeploys.

## Repository

[github.com/MohanRajS-01/mec](https://github.com/MohanRajS-01/mec)
