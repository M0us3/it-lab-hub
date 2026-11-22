# IT Lab Hub

A static, dark-themed IT learning dashboard designed for GitHub Pages.

## Publish with GitHub Pages
1. Create a new GitHub repository (for example `it-lab-hub`).
2. Upload the contents of this folder to the repository root. Keep `index.html`, `assets/`, and `data/` in their current locations.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site. The Pages URL will appear in that settings panel.

## Features
- Screenshot-inspired dark dashboard, sidebar, technology tiles and quick links.
- Search across resource titles, topics, descriptions, source and type.
- Topic navigation, resource type and difficulty filters.
- Completion checkboxes saved locally in the current browser using localStorage. No account, backend or sync.
- Edit `data/resources.json` to add, remove or update curated links.

## Add a resource
Add an object to `data/resources.json` with these fields:
`title`, `topic`, `type`, `level`, `duration`, `source`, `url`, `desc`.
Optional: `"featured": true`.

Allowed topic names initially: Azure, AWS, Entra ID, Exchange, Storage, VMware, Security, Intune, PowerShell, Active Directory.

## Curated source notes
The catalogue prioritizes hands-on Microsoft Learn modules and guided projects, MicrosoftLearning lab repositories, official AWS workshops, VMware Hands-on Labs, and PowerShell-focused training.

Some labs require an eligible tenant, subscription, licensed products, local VMs or paid cloud resources. Check prerequisites and estimated costs before launching. Microsoft Learning repositories may be instructor-oriented and may require separate lab environments. AWS workshops and VMware HOL may have account/access requirements.

## Local preview
Open `index.html` through a local static server (recommended) or publish through GitHub Pages. `fetch()` for the JSON catalogue may not work when opening the file directly with a `file://` URL.

## No secrets
Do not commit credentials, API keys, tenant identifiers, private IP details or sensitive lab configuration to a public repository.
