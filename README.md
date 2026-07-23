# Shailesh Alagan — Portfolio Website

A single, self-contained personal portfolio site. Everything (styles, scripts,
icons) lives inside `index.html` — no build step, no installs. Just open it or
upload it.

---

## 1. Quick start (preview it)

**Double-click `index.html`** — it opens in your browser. That's it.

Everything already works. The extra files below (photo, resume, screenshots)
are **optional** — the page looks complete without them and shows clean
placeholders where a file is missing.

---

## 2. Folder structure — where everything goes

Put these next to `index.html`. Create the `certs` and `shots` folders yourself.

```
portfolio/
├── index.html          ← the whole website (already done)
├── README.md           ← this file
├── photo.jpg           ← your headshot (hero photo)   [optional]
├── resume.pdf          ← your resume (Résumé buttons)  [optional]
├── certs/              ← certificate & diploma PDFs    [optional]
│   ├── administrator.pdf
│   ├── app-builder.pdf
│   ├── harvardx-data-science.pdf
│   └── csun-diploma.pdf
└── shots/              ← project screenshots           [optional]
    ├── emr/
    │   ├── emr1.png
    │   ├── emr2.png
    │   ├── emr3.png
    │   └── emr4.png
    ├── marketing.png
    └── ... (see table below)
```

> Filenames must match **exactly** (lowercase, same spelling). If a file is
> missing, that piece just doesn't show — nothing breaks.

---

## 3. Your photo

- Save it as **`photo.jpg`** next to `index.html`.
- A **square or portrait** crop looks best (the frame is 260×320 and auto-crops).
- Until you add it, an "SA" monogram shows in the frame.

---

## 4. Resume

- Save it as **`resume.pdf`** next to `index.html`.
- The "Résumé ↓" buttons in the hero and Contact section open it.

---

## 5. Certificates & diploma (`certs/` folder)

Create a folder named `certs` and drop these PDFs in:

| Link on site | Filename |
| --- | --- |
| Salesforce Certified Administrator | `certs/administrator.pdf` |
| Salesforce Certified Platform App Builder | `certs/app-builder.pdf` |
| HarvardX Data Science (9-course series) | `certs/harvardx-data-science.pdf` |
| CSUN diploma ("View diploma") | `certs/csun-diploma.pdf` |

- **HarvardX = 9 courses:** merge the 9 course PDFs into one `harvardx-data-science.pdf`
  (any free "merge PDF" tool), or replace the link with your edX verification URL.
- Platform Developer I has no link yet (marked "Expected 2026").
- Check each PDF for personal info before making the site public.

---

## 6. Project screenshots (`shots/` folder)

Create a folder named `shots`. Screenshots appear **inside a project's
"Technical details"** when someone expands it. Use `.png`, and **blur any real
customer data** first.

| Project | Filename |
| --- | --- |
| AI Lead Outreach Platform | `shots/ai-outreach.png` |
| Marketing Attribution | `shots/marketing.png` |
| Expense Reconciliation | `shots/expense.png` |
| Electronic Medical Records (EMR) | `shots/emr/emr1.png` |
| Electronic Medical Records (EMR) | `shots/emr/emr2.png` |
| Electronic Medical Records (EMR) | `shots/emr/emr3.png` |
| Electronic Medical Records (EMR) | `shots/emr/emr4.png` |
| Salesforce CRM Implementation | `shots/crm/crm1.png` |
| Salesforce CRM Implementation | `shots/crm/crm2.png` |
| Salesforce CRM Implementation | `shots/crm/crm3.png` |
| Salesforce CRM Implementation | `shots/crm/crm4.png` |
| Call Center Analytics | `shots/call-center.png` |
| Sales / ROI / Executive Dashboards | `shots/dashboards.png` |
| Lead Intake & Routing | `shots/lead-intake.png` |
| Social Lead Ads Processor | `shots/social-leads.png` |
| Appointment Sync Service | `shots/appointment-sync.png` |
| Co-op Marketing Automation | `shots/coop.png` |
| Travel Management Platform | `shots/traform.png` |

You only need the ones you have — the rest stay hidden.

---

## 7. Text to fill in (edit `index.html`)

Open `index.html` in any text editor and search (Ctrl+F) for:

- Trailhead profile is set to `https://www.salesforce.com/trailblazer/shaileshalagan`.
- **`og:image`** (in the `<head>`) → after you deploy, change `photo.jpg` to the
  **full URL**, e.g. `https://yourdomain.com/photo.jpg`. LinkedIn needs the full
  URL to show your photo when the link is shared. (Also add an `og:url` line with
  your live address.)

Everything else — name, contact, experience, education, certs — is already filled in.

---

## 8. How to edit content

- **Text:** open `index.html` in a text editor (VS Code, Notepad++, even Notepad),
  find the words, change them, save. Refresh the browser.
- **Add a project:** copy any `<article class="proj" ...> ... </article>` block,
  paste it, change the number in `data-num` and in `<div class="proj-num">`, set
  `data-cat` to `salesforce`, `fullstack`, or `automation`, and edit the text.
- **Theme, filters, "Show all", back-to-top, etc.** all work automatically — no
  edits needed.

---

## 9. Go live (free hosting)

Pick one:

### Option A — Netlify (easiest, no coding)
1. Put `index.html` + your files in one folder.
2. Go to **app.netlify.com** and sign up (free).
3. **Drag the whole folder** onto the page → it's instantly live at a
   `something.netlify.app` link.
4. To update later, drag the folder again.

### Option B — GitHub Pages
1. Create a GitHub repo, upload all the files.
2. Repo **Settings → Pages** → set branch to `main` / root → Save.
3. Live at `https://yourusername.github.io/reponame/`.

---

## 10. Custom domain (optional, ~$10–15/year)

1. Buy a domain from **Cloudflare**, **Namecheap**, or **Porkbun**
   (e.g. `shaileshalagan.com`). Avoid GoDaddy.
2. In your host (Netlify / GitHub Pages), open **Domain settings → Add custom
   domain** and enter it.
3. Copy the DNS records it gives you into your registrar's DNS settings.
4. Wait a few minutes to a few hours. HTTPS is set up automatically and free.

---

## Notes

- The site works in **light and dark mode** (toggle in the top-right; it remembers
  your choice and follows the system default).
- **Save-as-PDF:** press **Ctrl+P** (Cmd+P on Mac) → "Save as PDF" to export the
  whole page; project details auto-expand in the export.
- No internet or server is required to view it locally — it's one HTML file.
