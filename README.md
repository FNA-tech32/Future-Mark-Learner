# Future Mark Learner

Future Mark Learner is an all-in-one cloud platform for coaching institutes. It helps non-technical institute owners manage students, teachers, attendance, exams, finances, SMS notifications, and student ID cards from one self-service, mobile-ready system.

This repository is the **marketing landing page** for Future Mark Learner. It is built for coaching centers in Bangladesh and supports English and Bengali.

## What the site includes

The landing page is a single scroll with these sections:

- **Hero** — headline, free-trial and demo calls to action, and a dashboard preview
- **Social proof** — animated counters and institutes using the platform
- **Features** — dashboard, student management, ID cards, attendance, exams, finance, SMS, and access control
- **Screenshots** — app previews for dashboard, students, ID cards, attendance, exams, finance, SMS, and mobile
- **Demo** — walkthroughs for the dashboard tour, student enrollment, and ID card generation
- **How it works** — create an institute, configure classes, enroll people, then run day-to-day work from one dashboard
- **Benefits** — why institutes switch from paper registers and spreadsheets
- **Roadmap** — planned product versions
- **Pricing** — Starter (৳500/month), Professional (৳1,500/month), and Enterprise (৳3,000/month), with a yearly toggle. Prices are in BDT
- **FAQ** — common questions about setup, skills, attendance, SMS, security, and mobile use
- **Call to action** — 14-day free trial
- **Contact** — Future Mark Learner customer support for institutes in Bangladesh, in English and Bengali

## Tech stack

- **Framework:** Next.js 16 (App Router, Turbopack)
- **Language:** TypeScript
- **UI:** React 19, Tailwind CSS v4, Lucide icons
- **Animation:** Framer Motion, GSAP, Lenis (smooth scroll)
- **3D:** Three.js via `@react-three/fiber` and `@react-three/drei`
- **Theming:** `next-themes`

## Getting started

Install dependencies and start the development server:

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Scripts

| Script | Description |
| --- | --- |
| `npm run dev` | Start the Next.js dev server with Turbopack |
| `npm run build` | Build the production bundle |
| `npm run start` | Run the production build locally |
| `npm run lint` | Lint the project with ESLint |

## Project structure

```
src/
├── app/                  # Layout, landing page, sitemap, robots
├── components/
│   ├── animations/       # Scroll reveal
│   ├── layout/           # Navbar and footer (brand + contact)
│   ├── sections/         # Hero, features, pricing, FAQ, CTA, and the rest
│   ├── three/            # Hero background scene
│   └── ui/               # Counters and device frames
└── lib/                  # Shared utilities
public/                   # Icons, manifest, and static assets
```

## Environment variables

Create a `.env.local` file in the project root:

```bash
NEXT_PUBLIC_SITE_URL=https://futuremarklearner.com
NEXT_PUBLIC_APP_URL=https://app.futuremarklearner.com
```

`NEXT_PUBLIC_SITE_URL` is used for SEO metadata, canonical URLs, Open Graph tags, `robots.txt`, and `sitemap.xml`. If it is not set, the site falls back to `https://futuremarklearner.com`.

`NEXT_PUBLIC_APP_URL` is the destination for **Get Started** and **Start Free Trial**. If it is not set, those buttons stay on the page.

## Contact

| | |
| --- | --- |
| Name | Future Mark Learner |
| Support | Customer support |
| Languages | English and Bengali |
| Region | Bangladesh |

The same details appear in the site footer (`#contact`) and in the page’s organization structured data.

## Deployment

The project is set up for [Vercel](https://vercel.com). Push to the main branch for a production deployment, or open a pull request for a preview.

Set `NEXT_PUBLIC_SITE_URL` and `NEXT_PUBLIC_APP_URL` in the Vercel project before a production deploy.

## License

Proprietary — all rights reserved.
