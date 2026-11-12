# Build, Ship, Win

A single-page website that lays out three software tools a solo developer could build and launch in 2026. It is a market analysis written as a polished, dark-themed landing page, not a working product.

## What it does

The page walks through three product ideas in the AI developer tooling space and ends with a verdict on which one to build first:

1. **LLM Radar**: an observability tool that tracks the cost, latency, token usage and error rate of every AI API call.
2. **MCP Hub**: a registry and directory for Model Context Protocol servers.
3. **ShieldReview**: an AI code review tool focused on security problems such as hardcoded secrets, injection flaws and auth bypasses.

Each idea has sections on the problem, the product, a sample usage snippet, revenue potential and a comparison with existing tools. A final section explains the order to build them in, so each product feeds the next.

## Tech stack

- Plain HTML, CSS and a small amount of vanilla JavaScript, all in one file (`index.html`)
- Google Fonts (Inter and JetBrains Mono), loaded from the web
- No build step, no dependencies, no backend

## Run it

Open `index.html` in a browser. Or serve the folder with any static server, for example:

```sh
python3 -m http.server 8000
```

Then visit http://localhost:8000. The site is fully static and needs no secrets, so you can host the folder as is on any static host (GitHub Pages, Vercel, Netlify). The `.vercel` entry in `.gitignore` suggests it was deployed on Vercel.

## Status

Working. It is a finished content page. The fonts and the social preview image load from external sites, so some styling needs an internet connection.

## Credits

The market analysis text was written with help from Claude, as noted in the page footer. The social preview image is an Unsplash photo linked by URL.
