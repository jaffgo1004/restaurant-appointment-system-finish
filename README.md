[README.md](https://github.com/user-attachments/files/25766146/README.md)
# 🍽️ The Velvet Room
### Private Fine Dining Reservation System

> BAI21113 Software Engineering Project · Raffles University · January 2026 Semester

A web-based reservation system for **The Velvet Room**, a private fine dining restaurant in Kuala Lumpur. The system allows customers to browse tasting menus, preview private suites, and submit reservations online — while giving staff a secure admin dashboard to manage all bookings.

---

## 👥 Team Members

| Name | Student ID | Role |
|------|------------|------|
| Lee Wen Xin | BIT_B2201F-2505004 | Lead Developer / Scrum Master |
| Jaff Go | BIT_A2201F-2501001 | Frontend Developer |
| Ngoi Chang Zen | BAI_B2009F-2601001 | QA / Tester |
| Lam Chuan Fong | BAI_B2009F-2601010 | Documentation Lead |

**Lecturer:** Azlina binti Adnan

---

## 🏛️ Private Dining Suites

| Suite | Capacity | Highlights |
|-------|----------|------------|
| Room 1 · The Crimson Suite | Up to 20 guests | Wine display, private AV system, floor-to-ceiling drapes |
| Room 2 · The Pearl Alcove | Up to 10 guests | Fresh florals, candlelit ambience, bespoke table setting |

---

## 🍴 Tasting Menus

| Menu | Price | Best For |
|------|-------|---------|
| The Executive Table | RM 388 / pax | Corporate dinners & business entertaining |
| The Anniversary Menu | RM 288 / pax | Anniversaries, proposals & date nights |
| The Family Feast | RM 218 / pax | Family gatherings & celebrations |
| The Celebration Dinner | RM 318 / pax | Birthdays & milestone celebrations |
| The Prestige Tasting | RM 688 / pax | Premium multi-course tasting experience |
| The Grand Brunch | RM 248 / pax | Weekend brunch & daytime occasions |

---

## ✨ Features

**Customer**
- Browse six tasting menus with course details and pricing
- Preview private suites with photos and amenities
- Select from 10 bookable time slots (11:00 AM – 9:00 PM)
- Submit reservations with real-time booking summary and estimated total cost
- Double-booking prevention — conflicts rejected automatically

**Admin Dashboard**
- Secure session-based login
- Visual room availability grid (Available / Booked) across all time slots
- View all reservations with full guest details
- Confirm or cancel reservations

---

## 🛠️ Technology Stack

| Layer | Technology | Justification |
|-------|------------|---------------|
| Backend | Python 3 + Flask | Lightweight, easy to set up, suitable for mid-sized web apps |
| Database | SQLite | File-based, zero configuration, appropriate for single-restaurant system |
| Frontend | HTML5 + Bootstrap 5 | Responsive grid, pre-built UI components, rapid development |
| Styling | Custom CSS | Bespoke luxury aesthetic using CSS variables and animations |
| JavaScript | Vanilla JS (ES6+) | No dependencies, fetch API for backend communication |
| Version Control | Git + GitHub | Team collaboration, branching, and code review |

---

## 🚀 Installation & Setup

### Prerequisites
- Python 3.x
- pip

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/LEEWXIN/restaurant-booking.git
cd restaurant-booking
```

**2. Install dependencies**
```bash
pip install flask
```

**3. Run the application**
```bash
python app.py
```

**4. Open in browser**
```
http://127.0.0.1:5000
```

### Default Admin Credentials
| Username | Password |
|----------|----------|
| `admin` | `admin123` |

---

## 📁 Project Structure

```
restaurant-booking/
├── app.py              # Flask application & API routes
├── database.py         # Database schema & seed data
├── restaurant.db       # SQLite database file
├── templates/
│   └── index.html      # Main HTML template (Jinja2)
└── static/
    ├── css/style.css   # Custom styles & luxury UI theme
    └── js/app.js       # Frontend logic & API calls
```

---

## 🔌 API Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/api/rooms` | Returns list of all rooms | No |
| GET | `/api/packages` | Returns list of all tasting menu packages | No |
| POST | `/api/reserve` | Submit a new reservation | No |
| POST | `/api/admin/login` | Admin authentication | No |
| POST | `/api/admin/logout` | Clear admin session | Yes |
| GET | `/api/admin/reservations` | Get all reservations | Yes |
| PATCH | `/api/admin/reservation/<id>` | Update reservation status | Yes |
| PATCH | `/api/admin/room/<id>` | Update room status | Yes |

---

## 🧪 Testing

Manual black-box testing across **12 test cases** covering:

| Area | Test Cases |
|------|-----------|
| Reservation submission | Valid submission, missing fields, double-booking prevention |
| Admin authentication | Valid login, invalid login |
| Admin dashboard | Cancel/confirm reservation, grid updates after booking |
| UI features | Menu detail preview, room preview modal, summary panel updates |
| Data integrity | 4:00 PM slot not available, data persists after server restart |

**Result: 12 / 12 test cases passed ✅**

---

## 📅 Agile Process (Scrum)

Development was organised into **3 Scrum sprints** over 6 weeks, with a Kanban board tracking progress across Backlog → In Progress → Review → Done.

| Sprint | Duration | Key Deliverables | Outcome |
|--------|----------|-----------------|---------|
| Sprint 1 | Week 1–2 | Project setup, DB design, Flask skeleton, basic reservation form | Core structure established |
| Sprint 2 | Week 3–4 | Full reservation flow, admin login, dashboard, room preview modal | Fully functional system |
| Sprint 3 | Week 5–6 | UI polish, time slots, menu previews, bug fixes, testing, docs | Production-ready system |

**Sprint completion rate: 10 / 10 user stories (100%) ✅**

---

## 🤝 Collaboration

- Feature branches for all major tasks (e.g. `feature/admin-dashboard`, `feature/reservation-form`)
- Pull requests submitted for code review before merging into `main`
- GitHub Issues used to track bugs and feature requests
- All four members contributed commits across different areas
- Daily updates via WhatsApp, weekly virtual sprint reviews

---

## 📄 Documentation

Full project report: [`SE_Project_Report_Final.docx`](./SE_Project_Report_Final.docx)
