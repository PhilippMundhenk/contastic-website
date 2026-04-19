> [!WARNING]
> **This repository has been archived.** Development continues in the monorepo at
> https://github.com/PhilippMundhenk/contastic (subdirectory `website/`).

# contastic-website

Marketing site for [Contastic](https://github.com/PhilippMundhenk/contastic) — the self-hosted, end-to-end encrypted address book.

Built with [Astro](https://astro.build) (static output). Deployed at `contastic.mundhenk.info`.

## Development

```bash
npm install
npm run dev       # Dev server on http://localhost:4321
npm run build     # Production build → dist/
npm run preview   # Preview the built site
```

## Deployment

Joins the Traefik network created by `contastic-server`:

```bash
docker compose up -d
```

The image is also published to `ghcr.io/philippmundhenk/contastic-website:latest` on every push via GitHub Actions.

## Related repositories

- [contastic-server](https://github.com/PhilippMundhenk/contastic) — FastAPI backend + deployment
- [contastic-web](https://github.com/PhilippMundhenk/contastic-web) — React web client
- [contastic-android](https://github.com/PhilippMundhenk/contastic-android) — Android app

See the [documentation wiki](https://github.com/PhilippMundhenk/contastic/tree/main/contastic-server/docs) for architecture and deployment details.
