[README.md](https://github.com/user-attachments/files/32474913/README.md)
# Converge 2026 — Event App
**Accion Labs · November 18–20, 2026 · Orlando, Florida**

An invitation-only event management web app for Accion Labs Converge 2026 — serving both event participants and the admin organizing team. Built as a Progressive Web App (PWA) so attendees can install it directly to their phone home screen without an App Store.

---

## 🚀 Live App

> URL will be added here once deployed to Vercel

---

## 📱 What's Inside

### Participant View
- **Home** — Event overview, countdown, quick access to all features
- **Agenda** — Full 3-day session schedule (Nov 18–20) with tracks and speakers
- **Q&A** — Submit and upvote questions for live sessions
- **Polls** — Vote in real-time polls and see live results
- **Notifications** — Push alerts from the event team
- **Feedback** — Rate sessions and submit NPS score
- **Profile** — Edit personal details and role

### Admin View (Event Organizing Team Only)
- **Dashboard** — Live KPIs, registrations, activity feed, countdown
- **Registration** — Manage attendees, confirm, waitlist, email
- **Agenda Builder** — Create and edit sessions across all 3 days
- **Q&A Moderation** — Pin, answer, or remove participant questions
- **Notifications** — Compose and send push notifications by audience segment
- **Feedback Analytics** — NPS scores, session ratings, export to CSV

---

## 🏗️ Current Status

| Layer | Status | Notes |
|---|---|---|
| Frontend UI | ✅ Complete | Full prototype — admin + participant |
| Login screen | ✅ Complete | Role selector — participant primary, admin secondary |
| PWA support | ✅ Complete | Installs to home screen on iOS and Android |
| Backend (Supabase) | 🔲 Pending | Week 1–8 engineering build |
| Real authentication | 🔲 Pending | Supabase Auth — magic link login |
| Live database | 🔲 Pending | PostgreSQL via Supabase |
| Push notifications | 🔲 Pending | OneSignal integration |

---

## 📁 Repository Structure

```
converge2026/
├── converge2026_app.html        ← Full app prototype (current)
├── README.md                    ← This file
└── converge2026_tech_spec.docx  ← Engineering handoff specification
```

> When the backend is added, the HTML file will be replaced by a Next.js project. The folder structure will expand to match the spec in `converge2026_tech_spec.docx`.

---

## 🖥️ Running Locally

No setup needed. Just open the file in any browser:

```bash
# Option 1 — Double-click the file
open converge2026_app.html

# Option 2 — Serve locally (optional, for PWA install testing)
npx serve .
# Then open http://localhost:3000
```

---

## ☁️ Deploying to Vercel

This repo is connected to Vercel for automatic deployment.

**Every push to `main` auto-deploys.** No manual steps needed.

To update content:
1. Edit `converge2026_app.html` directly in GitHub (click the file → pencil icon)
2. Commit the change
3. Vercel deploys automatically within 60 seconds

To set a custom domain (`converge.accionlabs.com`):
1. Go to Vercel → Project → Settings → Domains
2. Add `converge.accionlabs.com`
3. Add a CNAME record in your DNS pointing to `cname.vercel-dns.com`

---

## 📲 PWA — Installing on Mobile

Participants open the Vercel URL in their phone browser:

**Android (Chrome)**
- A banner appears automatically → tap **Install** or **Add to Home Screen**

**iPhone (Safari)**
- Tap the **Share** button (box with arrow)
- Tap **Add to Home Screen**
- Tap **Add**

The app installs with the Accion Labs icon, opens full-screen — no browser bar — identical to a native app. No App Store or Play Store needed.

---

## 🔧 Backend Upgrade Plan

The current version is a UI prototype with no live database. The backend will be added in an 8-week engineering build using:

| Service | Purpose |
|---|---|
| **Supabase** | Auth, PostgreSQL database, real-time Q&A, file storage |
| **Vercel** | Frontend hosting, CI/CD (already configured) |
| **OneSignal** | Push notifications to mobile and desktop |
| **Next.js 14** | Frontend framework replacing the single HTML file |

Full schema, architecture, and week-by-week delivery timeline are in `converge2026_tech_spec.docx`.

**The Vercel URL and custom domain stay the same when the backend is added.**

---

## ✏️ Making Content Changes (No Code Required)

To update session titles, speaker names, dates, or any text:

1. Open `converge2026_app.html` in GitHub
2. Click the **pencil icon** (Edit this file)
3. Use **Ctrl+F** (or Cmd+F) to find the text you want to change
4. Edit it
5. Click **Commit changes**
6. Vercel deploys the update automatically

---

## 🗓️ Key Dates

| Milestone | Date |
|---|---|
| Prototype live on Vercel | September 2026 |
| Backend engineering start | September 27, 2026 |
| App go-live (with real backend) | November 10, 2026 |
| **Converge 2026 — Day 1** | **November 18, 2026** |
| **Converge 2026 — Day 3** | **November 20, 2026** |

---

## 👥 Team

| Role | Owner |
|---|---|
| Creative Lead / UI Design | Abhijeet — Global Marketing, Accion Labs |
| Engineering Lead | TBD — assign at project kickoff |
| Event Management | Global Marketing Team, Accion Labs |

---

## 📄 Related Documents

| Document | Purpose |
|---|---|
| `converge2026_tech_spec.docx` | Full engineering specification — stack, schema, timeline, deployment |
| `converge2026_app.html` | Current prototype — complete UI for admin and participant |

---

*Accion Labs Converge 2026 · Global Marketing Team*
