# ToniPR

A static website and product-interface prototype for turning an interview into reusable marketing content. The experience connects product discovery, onboarding, interview preparation, and content review so a visitor can understand how one conversation could become several publishable formats.

The repository includes both the public-facing website and signed-in product screens. It is implemented with HTML, CSS, and JavaScript rather than a frontend framework.

## Explore the experience

- **Public site:** product story, pricing, FAQ, and example articles.
- **Getting started:** authentication, onboarding, and checkout screens.
- **Interview workflow:** preparation, interview, and previous-interview views.
- **Content workspace:** LinkedIn posts, X threads, blog articles, and founder-kit pages.
- **Account area:** profile, settings, and support.

These pages present the intended service journey. This source repository does not include an AI-generation backend, payment service, or authentication server, so the corresponding screens should be reviewed as prototype UI.

## Run locally

Use Python 3 to serve the files:

```sh
git clone https://github.com/anushaxrama/toniPR.git
cd toniPR
python3 -m http.server 8080 --bind 127.0.0.1
```

Open [localhost:8080](http://localhost:8080) for the public site or [dashboard.html](http://localhost:8080/dashboard.html) for the product workspace. There is no package-install or build step.

Some fonts and media use external resources, so their appearance depends on network availability.

## Implementation

| Location | Responsibility |
| --- | --- |
| `index.html` | Public landing page |
| `onboarding.html`, `interview.html` | Entry and interview flows |
| `dashboard.html` | Product overview |
| `linkedin-posts.html`, `x-threads.html`, `blog-articles.html` | Content-format views |
| `blog/` | Sample editorial pages |
| `css/` | Shared background, branding, and dashboard styles |
| `js/dashboard-shell.js` | Responsive navigation drawer |
| `assets/` | Product illustrations and media |

The interface uses a shared visual language across the marketing and product pages, including the Toni character, warm typography, and responsive navigation.

## Scope

This repository demonstrates the frontend and interaction design. It does not verify generated-content quality, account security, checkout completion, or real customer outcomes. Those require the corresponding application services and separate testing.
