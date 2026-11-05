# vetflow-demo-site

A static demo site for **Happy Claw Veteriner Kliniği**, a fictional pet
clinic in Girne (Kyrenia), TRNC — built to showcase
[VetFlow](https://github.com/KursatNurKutay/Vetflow) (a product of Koby
Soft) in a realistic clinic-website setting, the same way
[dentflow-demo-site](https://github.com/KursatNurKutay/dentflow-demo-site)
does for DentFlow with Dr. Aslan Diş Polikliniği.

This is separate from
[vetflow-web-page](https://github.com/KursatNurKutay/vetflow-web-page),
which is reserved for VetFlow's actual marketing site (`vetflowclinic.com`)
— the same split that keeps `dentflow-demo-site` separate from
`dentflow-web-page` (`dentflowclinic.com`).

## What's here

- `index.html` — single-page site: hero, clinic intro, services, vet team,
  "why us", hours/location, FAQ, contact.
- `css/styles.css` — styling, no build step, no framework. Same design
  system/structure as the Dentflow demo site, reskinned green for a
  pet-care feel (not a literal copy — independent files, same patterns).
- `favicon.svg` — paw-print icon.
- `assets/img/` — clinic/vet photo slots (see that folder's `README.md`).
  Empty slots fall back to a CSS placeholder rather than a broken image.

No build tooling, no dependencies — open `index.html` directly in a
browser to preview.

## Content source

The clinic identity (name "Happy Claw", test-clinic flag, Turkish staff
language) comes from the seed data in the
[Vetflow](https://github.com/KursatNurKutay/Vetflow) backend repo
(`backend/prisma/seed.ts`), which also names the intended chat subdomain
`happyclaw.testsitehub.com` once the widget is live. Address, vet names,
hours, services, and FAQ content are fictional, grounded in a quick look
at real TRNC/Turkish vet clinic naming and service conventions — not
copied from any real clinic.

## No chat widget yet

Unlike the DentFlow demo (which embeds a working widget), this site does
**not** embed a VetFlow chat widget. As of this build, VetFlow has no
deployed backend — per `docs/phase-1-keys.md` in the Vetflow repo, Railway
deployment is Phase 8 and hasn't happened yet, so there's no real widget
script URL or widget key to embed. The demo banner and the "assistant
hint" section both say the chat integration is coming soon rather than
claiming one works.

Once VetFlow is deployed and a widget key exists for the Happy Claw test
clinic (the equivalent of `docs/embed.md` in the Dentflow repo), add the
widget `<script>` tag at the end of `<body>` in `index.html`, same as the
Dentflow demo site, and update the demo banner / assistant-hint copy to
match.

## Deployment

Not yet deployed. Following the same pattern as the Dentflow demo
(`draslandis-demo.testsitehub.com` on Vercel, DNS at Hostinger), this is
intended for a `testsitehub.com` subdomain once ready to go live.
