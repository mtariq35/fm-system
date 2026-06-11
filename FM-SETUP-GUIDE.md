# Facility Management System — Phase 1
## Complete Setup & User Guide

**Prepared for:** Muhammad Tariq, Facility Manager  
**Version:** 1.0 | **Date:** June 2026

---

## WHAT'S INCLUDED IN PHASE 1

| File | Purpose | Used By |
|---|---|---|
| `visitor-feedback.html` | QR feedback form for visitors | Visitors / Clients |
| `supervisor-dashboard.html` | Live complaints dashboard | Supervisors (x3) |
| `manager-analytics.html` | Analytics, reports & KPIs | Muhammad (Manager) |
| `qr-generator.html` | Generate & print QR posters | Muhammad (Manager) |

---

## HOW THE SYSTEM WORKS

```
Visitor scans QR code
        ↓
Opens visitor-feedback.html on their phone
        ↓
Selects floor → area → rating → issue → comment / photo / voice
        ↓
Submits feedback (reference number shown)
        ↓
Appears instantly on supervisor-dashboard.html
        ↓
Supervisor assigns → updates status → resolves
        ↓
Muhammad reviews analytics on manager-analytics.html
```

---

## OPTION A — USE RIGHT NOW (Local / Demo Mode)

All 4 files work immediately when opened in a browser.
They share data via the browser's localStorage.

**Steps:**
1. Open all 4 files in Chrome or Edge
2. Use `qr-generator.html` to generate QR posters
3. Open `supervisor-dashboard.html` on your team's devices
4. Open `manager-analytics.html` for your own view
5. Scan a QR or open `visitor-feedback.html` to test

> ⚠️ In local mode, all files must be on the SAME device/browser
> to share data. For real multi-device use, see Option B.

---

## OPTION B — GO LIVE (Recommended for Real Use)

To use across multiple devices (phones, tablets, computers),
host the files on a web server. Free options:

### Easiest: Netlify Drop (free, 2 minutes)
1. Go to **https://app.github.com**
2. Drag and drop all 4 HTML files into the browser
3. Netlify gives you a live URL like:
   `https://mtariq35.github.io/fm-system`
4. Share that URL with your team

### After hosting:
1. Open `qr-generator.html`
2. Update the **Feedback URL** field to:
   `https://mtariq35.github.io/fm-system/visitor-feedback.html`
3. Regenerate all QR codes
4. Print and post the new posters

> ✅ Once hosted, all devices share the same data in real time.

---

## STEP-BY-STEP: GENERATING & POSTING QR CODES

1. Open `qr-generator.html`
2. Enter your live feedback URL in the URL field
3. Select your floor (5th Floor, 4th Floor, or Common Areas)
4. Tick the locations you want QR codes for
5. Click **⚡ Generate QR Codes**
6. Click **🖨 Print** on each poster, or **Print All** for batch
7. Print on A5 paper (or A4, scaled)
8. Laminate and post in each location

**Recommended locations to start:**
- Male & Female washrooms (5th and 4th floor)
- Breakout areas
- Reception desks
- Prayer rooms

---

## USER ROLES & ACCESS

### Visitors / Clients
- Scan QR code → feedback form opens automatically
- No login required
- English / Arabic language toggle
- Can rate, select issues, comment, upload photo, use voice, leave contact

### Supervisors (x3)
- Open `supervisor-dashboard.html` in browser
- Select their name from the login screen
- See all incoming complaints in real time
- Assign, update status, add notes

### Facility Manager (Muhammad)
- Open `manager-analytics.html` for full analytics
- Or open `supervisor-dashboard.html` → login as "Facility Manager (Muhammad)"
- View all supervisor activity
- See KPIs, trends, ratings, location breakdown
- Generate and print daily/weekly AI reports

---

## COMPLAINT LIFECYCLE

```
OPEN → ASSIGNED → IN PROGRESS → VERIFIED → CLOSED
```

| Status | Who Acts | What It Means |
|---|---|---|
| Open | — | Just received, not yet assigned |
| Assigned | Supervisor | Allocated to a team member |
| In Progress | Supervisor | Team actively working on it |
| Verified | Supervisor | Solution has been verified |
| Closed | Supervisor | Fully resolved and closed |

---

## ANALYTICS & REPORTS

Muhammad's analytics dashboard shows:

- **KPIs:** Total complaints, resolution rate, avg time, open count
- **Trend chart:** 7-day complaint volume line graph
- **Rating donut:** Good / Neutral / Bad breakdown
- **Top locations:** Bar chart of highest complaint areas
- **Issue categories:** Cleaning, Damage, Safety, Supplies %
- **Supervisor table:** Performance per supervisor
- **AI Report:** Auto-generated narrative summary

**Period filter:** Today / Week / Month

**To print a report:**
1. Open `manager-analytics.html`
2. Select period (Today / Week / Month)
3. Click **View Full Report** or **🖨 Print**
4. Print or save as PDF

---

## VOICE FEEDBACK (VISITOR FORM)

Visitors can speak their feedback instead of typing:

1. Tap the 🎤 **Voice** button next to the comments box
2. Allow microphone permission when prompted (first time only)
3. Speak naturally
4. Text appears automatically in the comments field
5. Tap again to stop, or it stops after a pause

**Language:** Automatically switches to Arabic when Arabic mode is selected.

**Supported browsers:** Chrome (Android/Desktop), Edge, Safari (iOS 14.5+)

---

## LOCATIONS COVERED — PHASE 1

**5th Floor (25 locations)**
Male Washroom, Female Washroom, Breakout Area, Reception,
Meeting Rooms 1–7, Male Prayer Room, Female Prayer Room,
HR Area, Finance Area, Procurement Area, OC Area, IT Area,
Library Area, Training Room, Executive Area, Design Team Area,
Strategy Team Area, Auditorium, Other Areas

**4th Floor (16 locations)**
Male Washroom, Female Washroom, Breakout Area, Reception,
Classrooms 1–8, Mother Room, Studio, Focus Room, Other Areas

**Common Areas**

**Total: 42 QR codes available**

---

## PHASE 2 ROADMAP (Coming Next)

| Phase | Module | Status |
|---|---|---|
| ✅ Phase 1 | QR Feedback System | Complete |
| 🔲 Phase 2 | Maintenance & Work Orders | Next |
| 🔲 Phase 3 | Health & Safety Incidents | Planned |
| 🔲 Phase 4 | Inspections & Audits | Planned |
| 🔲 Phase 5 | Contractor Management | Planned |
| 🔲 Phase 6 | Project Management | Planned |
| 🔲 Phase 7 | Environmental & Sustainability | Planned |

---

## SUPPORT & CHANGES

Any changes, additions, or new modules — share with Claude and
they will be implemented. Common requests:

- Add new locations
- Change language text
- Add new issue categories
- Modify the complaint workflow
- Add email/WhatsApp notifications
- Connect to a real database

---

*FM System Phase 1 | Built by Claude (Anthropic) for Muhammad Tariq*
