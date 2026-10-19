# Be Human (behmn.ai) — Build Checklist

How we work: finish a phase, then **quality-check it on the live Netlify site** before starting the next one.
Each phase ends with a QC gate. Nothing in the next phase starts until that gate is ticked.

Live site: https://newappli.netlify.app/ · Deploys from the `main` branch.

---

## Phase 0: Themes and responsive layout ✅ built, awaiting your QC
- [x] Landing page: hero, services, approach, about, contact form, footer
- [x] Light, dark and system themes (switch in the header, remembered on later visits)
- [x] System theme follows the device's light/dark setting live
- [x] Text and button colors pass WCAG AA contrast in both themes
- [x] Responsive on phones (280px+), tablets and desktops; no sideways scrolling
- [x] Phone menu (hamburger) with all links; closes on link tap, outside tap or Escape
- [x] Touch-friendly tap targets on phones and tablets
- [x] Form fields don't trigger iPhone zoom-in
- [x] Menu links scroll to sections without hiding them under the header
- [ ] **QC gate:** check themes and layout on your phone, a tablet and a computer

## Phase 1: Fixes and essentials
- [ ] Branded "thank you" page after the contact form is sent (instead of Netlify's default)
- [ ] Confirm form submissions arrive in Netlify → Forms; set up email notification
- [ ] Custom 404 (page not found) page
- [ ] "Skip to content" link for keyboard and screen-reader users
- [ ] Link previews for LinkedIn, texts and Slack (Open Graph image, title, description)
- [ ] Favicon set for iPhone home screen and Android (apple-touch-icon, web manifest)
- [ ] Replace text-character icons with proper SVG icons (consistent on every device)
- [ ] **QC gate:** send a test form, share the link somewhere to see the preview, try a bad URL

## Phase 2: Your real brand and content
- [ ] Official Be Human colors, fonts and logo (from behmn.com or brand files you supply)
- [ ] Final headline, intro and service descriptions in your own words
- [ ] Founder / team section with photo and short bio
- [ ] Contact details: email, LinkedIn, location / service area
- [ ] Privacy policy page (needed for the contact form and, later, logins)
- [ ] **QC gate:** read every line on the live site; confirm it sounds like you

## Phase 3: Credibility, conversion and launch polish
- [ ] Testimonials and/or client logos
- [ ] 2–3 short case studies (problem → approach → result)
- [ ] Booking link (e.g. Calendly or Cal.com) on "Book a conversation"
- [ ] Subtle scroll-in animations (respecting reduced-motion settings)
- [ ] SEO: page titles, descriptions, sitemap.xml, robots.txt, structured data
- [ ] Speed pass: Lighthouse score 90+ on mobile and desktop
- [ ] Privacy-friendly analytics (e.g. Netlify Analytics, Plausible)
- [ ] Connect the custom domain `behmn.ai` in Netlify with HTTPS
- [ ] **QC gate:** run Lighthouse; book a test meeting; visit via behmn.ai

## Phase 4: Supabase database and login (last)
Only once the site is as functional as possible without it.
- [ ] Connect the site to your Supabase project (public keys only in the browser)
- [ ] Save contact form submissions to a Supabase table (with row-level security)
- [ ] Email login (magic link or password) via Supabase Auth
- [ ] Client area: a members-only page that logged-in clients can see
- [ ] Admin view of form submissions / leads (restricted to you)
- [ ] Security review: row-level security policies, no secret keys in the site code
- [ ] **QC gate:** sign up, log in, log out, submit a form, and confirm data is stored only where it should be
