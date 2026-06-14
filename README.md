# PropFlow 🏠
### PG Property Management System

> One platform for Owners, Tenants, and Workers — manage everything from rent to repairs, without WhatsApp chaos.

🔴 **Live Demo:** [https://demo-ofi9.onrender.com](https://demo-ofi9.onrender.com)

---

## The Problem It Solves

Managing a PG property today means:
- Rent reminders scattered across WhatsApp
- No record of who paid and who didn't
- Maintenance workers with no task tracking
- Vacate requests lost in chat threads
- Owners with no clear view across multiple properties

**PropFlow replaces all of that with one organized system.**

---

## Who Uses It

| Role | What They Can Do |
|------|-----------------|
| 🏢 **Owner** | Add properties, assign tenants, view payment ledger, get alerts, manage vacate requests |
| 🧑 **Tenant** | View rent due, make payment entries, chat with owner, submit vacate form |
| 🔧 **Worker** | Receive maintenance tasks, update job status, view assigned property |

---

## Features

### 💰 Payment Ledger
- Monthly rent tracking per tenant
- Payment status: Paid / Pending / Overdue
- Full history per tenant and per property
- Summary view for owner across all units

### 💬 Internal Chat
- Direct messaging between Owner ↔ Tenant
- Owner ↔ Worker communication
- No need for WhatsApp — all conversations stay inside the platform

### 🔔 Alerts & Notifications
- Rent due reminders
- Maintenance task updates
- Vacate request status changes

### 📋 Vacate Management
- Tenant submits vacate form with notice period
- Owner reviews and approves/rejects
- Tracks move-out date and dues clearance

### 🏘️ Multi-Property Support
- Each property managed independently
- Separate tenant list, worker list, and ledger per property
- Owner dashboard shows all properties at a glance

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Flask |
| Frontend | HTML5, CSS3, JavaScript |
| Database | SQLite / PostgreSQL |
| Deployment | Render |
| Version Control | Git, GitHub |

---

## Project Structure

```
propflow/
├── app.py                  # Main Flask application
├── models/
│   ├── owner.py
│   ├── tenant.py
│   ├── worker.py
│   └── payment.py
├── routes/
│   ├── auth.py
│   ├── dashboard.py
│   ├── payments.py
│   ├── chat.py
│   └── vacate.py
├── templates/
│   ├── owner/
│   ├── tenant/
│   └── worker/
├── static/
│   ├── css/
│   └── js/
└── requirements.txt
```

---

## Getting Started

### Prerequisites
- Python 3.9+
- pip

### Installation

```bash
# Clone the repo
git clone https://github.com/vikasvijay246-sys/profly-B.git
cd profly-B

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

App runs at `http://localhost:5000`

### Default Login (Demo)

| Role | Email | Password |
|------|-------|----------|
| Owner | owner@demo.com | demo123 |
| Tenant | tenant@demo.com | demo123 |
| Worker | worker@demo.com | demo123 |

---

## Screenshots

> *(Add screenshots here — Owner Dashboard, Tenant Ledger, Chat View, Vacate Form)*

```
Tip: Use Ctrl+Shift+S or Snipping Tool → upload to /static/screenshots/ → link here
```

---

## Key Learnings

- Designed a **multi-role authentication system** from scratch using Flask sessions
- Built a **real-time-style chat** feature using polling without WebSockets
- Structured a **relational data model** linking owners → properties → tenants/workers
- Handled **payment state logic** (paid/pending/overdue) with automated monthly resets
- Deployed and maintained a **live production app** on Render with zero downtime

---

## Future Improvements

- [ ] SMS/Email rent reminders via Twilio / SendGrid
- [ ] PDF rent receipt generation
- [ ] Mobile-responsive redesign
- [ ] UPI payment integration
- [ ] WhatsApp notification via API

---

## Author

**M. Vijay Kumar**
- GitHub: [@vikasvijay246-sys](https://github.com/vikasvijay246-sys)
- LinkedIn: [vijay-kumar-murgani](https://linkedin.com/in/vijay-kumar-murgani)
- Email: vijaykumarmurgani@gmail.com

---

> Built with Python & Flask. Deployed live. Built to solve a real problem.
