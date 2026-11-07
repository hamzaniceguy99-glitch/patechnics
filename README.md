# PA Technics — electrical installation & charging

Static marketing site (HTML / CSS / JS, no build step) hosted on GitHub Pages
at `patechnics.shop`.

> Generated from `C:\Users\souha\coaching-sites-factory` (content file `sites/patechnics.mjs`).
> To change the content, edit that file and run `node build.mjs patechnics` — editing the
> HTML here directly would be overwritten on the next build.

## Before you promote this site

| Priority | What | Where |
|---|---|---|
| 🔴 Blocking | Legal page: fill every `[BRACKET]` (legal name, address, state, payment provider). Have a lawyer review it if you can. | `legal.html` |
| 🟠 Important | `contact@patechnics.shop` doesn't exist yet: set up free email forwarding in Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Contact form: replace `VOTRE_ID_FORMSPREE` with your Formspree id (until then it falls back to `mailto:`). | `contact.html` |
| 🟠 Important | Add a real introduction of the coach (name, background, photo). Never invent credentials. | `about.html` |
| 🟡 Later | Prices ($Quote / $Quote / $Declined) and plan contents should match what you actually sell. | `index.html` `#pricing` |
| 🟡 Later | Testimonials: only add real ones, with permission. Fake reviews are illegal (FTC). | — |

## Business description (Stripe, directories…)

```
We are PA Technics, an electrical installation business in Wevelgem in West Flanders, trading since June 2023. We install charge points and charging infrastructure, carry out general electrical installation work, and deal with connection capacity. There is one thing about charging in Flanders that decides most of what it costs, and it is not the price of electricity. Part of the distribution charge for customers with a digital meter is based on the monthly peak, measured as the highest quarter-hour average in that month and then averaged across the preceding twelve months, with a floor of two and a half kilowatts. A single charging session taken at full power while the oven and the heat pump are running sets a peak that then sits in that twelve-month average. So the cost comes from how fast the energy is drawn rather than how much of it is used, and dynamic load balancing that modulates against the whole building is not a comfort option. Separately, a charger can produce smooth DC residual current capable of blinding an ordinary type A device, so protection must be type B or type A with six milliamp DC detection. Site: patechnics.shop
```

## Structure

```
index.html            Home: hero, programs, method, pricing, approach, FAQ
programs.html         The four programs in detail
about.html            How we work, principles
contact.html          Contact form
legal.html            Business info, privacy policy, terms of service
404.html              Error page (absolute paths)
assets/css/style.css  Brand colors at the top, shared styles below
assets/js/main.js     Menu, theme, animations, form
```

## DNS (Namecheap → Advanced DNS)

Delete the parking records, then add:

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
