# Claude Artifact Website

This folder is a regular static website for the published Claude artifact:

<https://claude.ai/public/artifacts/e31ed19f-f7ec-4c3e-8701-c9f792ef9321>

## Deploy

No build step is required. Deploy the `artifact-site/` directory as the publish directory on any static host.

Examples:

- **Netlify:** drag `artifact-site/` into the Netlify deploy UI, or set publish directory to `artifact-site`.
- **Vercel:** create a static project and set output/publish directory to `artifact-site`.
- **Cloudflare Pages:** use no build command and set output directory to `artifact-site`.
- **GitHub Pages:** publish the contents of this directory from the configured Pages branch.

## Connect a domain

1. Add your custom domain in your host dashboard.
2. Copy the host-provided DNS records into your domain registrar.
3. Typical records are:
   - `CNAME www -> <host-provided target>`
   - `A @ -> <host-provided IP>` or ALIAS/ANAME if your registrar supports it
4. Wait for DNS propagation, then enable/verify HTTPS in the host dashboard.

If you know the exact domain and host, replace the placeholder DNS values in `index.html` with the real records.
