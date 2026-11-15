# Abed Gazi

**Software engineer — Python, full-stack web, and automation.**
Final-year B.Sc. Computer Science & Engineering student at North South University, Dhaka.

I build systems that work end to end and I measure them. My fraud-detection pipeline
went from 0.27% to 25.4% precision. My Linux monitor makes 4.8× fewer system calls than
the naive version, and a built-in check proves the readings are identical. I've also
shipped a production web platform for an enterprise IT company in Dhaka.

---

### Selected work

**[SentryWatch](https://github.com/abed101-glitch/sentrywatch)** · Python · FastAPI · scikit-learn · n8n
Event-driven fraud detection pipeline. Transactions arrive at an n8n webhook. A FastAPI
service scores them with an Isolation Forest plus per-account behavioural baselines
(Welford + EWMA, velocity checks). High-severity events trigger throttled Telegram alerts
and are logged to Google Sheets.
- Precision **0.27% → 25.4%** and false alarms per real fraud **370 → 2.9** on 284,807 real transactions
- Per-account baselines cost **0.008 ms per transaction** and **127 bytes per account**
- **96 tests** covering the baseline store and the alerting logic

**[sysmon](https://github.com/abed101-glitch/sysmon)** · C · Linux · procfs
A system monitor built on raw system calls, implemented twice so the cost of the careless
version can be measured.
- **4.8× fewer syscalls, 3.3× faster**, verified with `strace` comparisons
- Verification mode proves both implementations report identical readings

**OMNI Systems platform — [omni.com.bd](https://omni.com.bd)** · React · Node.js · Express · MongoDB
Production website and web platform for an enterprise IT company that has served banks,
government and corporate clients since 2004. It has a public site, customer accounts with
ordering, consultation booking, and an admin panel for products, orders, leads and staff.
- JWT auth, bcrypt, role-based admin, image uploads via Cloudinary, email notifications
- Deployed across cPanel (front end), Render (API) and MongoDB Atlas, with uptime monitoring
- *Private repository: company code*

**Mimosa Organic Solution: e-commerce store** · Next.js 16 · TypeScript · Prisma · PostgreSQL
Freelance build of a full store with an admin panel covering orders, stock, reviews, delivery zones and content.
- Transactional ordering: order, line snapshots, stock decrement and cart clear in one DB transaction
- Signed DB-backed sessions, `scrypt` passwords, path-traversal-safe media serving
- Payment adapter layer: cash on delivery live, SSLCommerz/bKash ready to switch on
- *Private repository: client code*

**FloodSight** *(in progress: senior design, NSU)* · PyTorch · segmentation-models · rasterio
Flood-extent mapping from Sentinel-1 SAR imagery (Sen1Floods11). Compares an Otsu baseline
against U-Net segmentation using SAR, permanent-water and DEM/slope inputs, focused on Bangladesh floods.

---

### Tech I use

| Area | Tools |
|---|---|
| Languages | Python, JavaScript, TypeScript, C, SQL |
| Back end | FastAPI, Node.js, Express, Prisma, REST APIs, JWT |
| Front end | React, Next.js, Vite, Tailwind CSS |
| Data & ML | scikit-learn, pandas, NumPy, PyTorch |
| Databases | PostgreSQL, MongoDB, SQLite |
| Automation | n8n, webhooks, Telegram Bot API, Google Sheets API |
| Deployment | Render, Railway, cPanel, Docker, Git, Linux |

---

### Certification

**Oracle Database Administration 2019 Certified Professional (OCP)** · Oracle

---

### Contact

🌐 [abed101-glitch.github.io](https://abed101-glitch.github.io) · 📧 gazi.abed@yahoo.com · 📍 Dhaka, Bangladesh · Open to on-site and remote roles
