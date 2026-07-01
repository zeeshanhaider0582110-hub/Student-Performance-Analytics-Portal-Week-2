# Student-Performance-Analytics-Portal-Week-2

A fully responsive front-end web application built using HTML5, CSS3, and JavaScript as part of a Web Development Internship — Week 2.

---

## 📌 Project Overview

EduTrack is a web-based Student Performance Analytics Portal designed to help educators and administrators monitor student academic performance, manage student records, and generate performance reports.


---

## 📄 Pages

| File | Page | Description |
|------|------|-------------|
| login.html | Login | Functional login form with validation and session authentication |
| index.html | Home | Welcome screen with animated stats, recent activity, and quick links |
| dashboard.html | Dashboard | Dynamic cards, animated counters, progress bars, and schedule |
| report.html | Performance Report | Grade distribution, subject scores, and term-by-term history |
| students.html | Student Records | Registration form, full table with search and filter functionality |
| about.html | About | Mission, platform stats, features, and team |
| contact.html | Contact | Contact form with validation and office information |

---


## ✅ Week 2 Requirements

- [x] Functional Login Form
- [x] Form Validation using JavaScript
- [x] Dynamic Dashboard Cards with animated counters
- [x] Student Information Tables — 11 columns
- [x] Search and Filter Functionality
- [x] Improved Mobile Responsiveness
- [x] Interactive Navigation Menu

---

## ⚙️ Features

*Authentication*
- Login form with email and password validation
- Show/hide password toggle
- Session-based auth using sessionStorage
- Auth guard on every page — redirects to login if not authenticated
- Sign Out button in sidebar on every page

*Navigation*
- Black left sidebar with active page highlighting
- Hover tooltips on each sidebar link
- Badge showing student count
- Mobile hamburger menu
- Mobile bottom navigation bar with 5 tabs
- Sidebar auto-closes after link click on mobile

*Dashboard*
- Animated number counters — count from 0 to real value on page load
- Animated progress bars and trend bars
- Color-coded stat cards with trend indicators

*Student Records Table*
- 10 students with full Pakistani names
- 11 columns — Name, ID, Department, Year, GPA, Attendance, Assignments, Phone, Status, Actions
- Live search bar — filters rows as you type
- Status chip filter buttons — All, Active, New, Warning, At-Risk
- Row highlight on search match
- Empty state message when no results found
- Record count updates dynamically
- Pagination bar

*Forms*
- Student registration form — 10 fields with live validation
- Contact form — 4 required fields with validation
- Login form — email format check, password length check
- Live error messages under each field
- Errors clear as you type

*Responsive Design*
- Mobile bottom navigation bar
- Sidebar slides in on mobile
- Grid stacks to single column on small screens
- Tables scroll horizontally on mobile

---

## 📁 Folder Structure


edutrack-portal/
├── login.html          # Login Page
├── index.html          # Home Page
├── dashboard.html      # Student Dashboard
├── report.html         # Performance Report
├── students.html       # Student Records
├── about.html          # About Page
├── contact.html        # Contact Page
├── css/
│   └── style.css       # All styles for entire project
└── js/
    ├── nav.js          # Sidebar, mobile menu, toast, modal helpers
    ├── dashboard.js    # Animated counters, progress bars, trend bars
    ├── students.js     # Registration form, search, chip filter
    └── contact.js      # Contact form validation


---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Page structure and semantic markup |
| CSS3 | Styling, Flexbox, Grid, animations, responsive design |
| JavaScript ES6 | Form validation, DOM manipulation, session auth, animations |
| Google Fonts — Inter | Professional typography |
| VS Code | Development environment |
| GitHub | Version control and project hosting |

---

## 🚀 How to Run

1. Download or clone this repository
2. Open the project folder in *VS Code*
3. Install the *Live Server* extension
4. Right-click login.html → *Open with Live Server*
5. Use the demo credentials to log in:
   - Email: zeeshan@edutrack.edu.pk
   - Password: edutrack2026

> No build tools, frameworks, or installations required. Pure HTML, CSS, and JavaScript.

---

## 🔐 Authentication Flow


login.html
    ↓  (enter credentials)
sessionStorage.setItem('loggedIn', 'true')
    ↓  (redirect)
index.html → dashboard.html → students.html → report.html
    ↓  (click Sign Out)
sessionStorage.removeItem('loggedIn')
    ↓  (redirect)
login.html


---

## 📊 Student Records Table

| Column | Description |
|--------|-------------|
| # | Row number |
| Student Name | Full name with email |
| Student ID | Format STU-2026-XXXX |
| Department | Enrolled department |
| Year | Academic year 1 to 4 |
| GPA | Color coded — green, amber, red |
| Attendance | Percentage |
| Assignments | Completed out of total |
| Contact | Phone number |
| Status | Active, New, Warning, At-Risk |
| Actions | View and Edit buttons |

---

## 📸 Screenshots

| Page | Preview |
|------|---------|
| Login | <img width="1916" height="946" alt="Screenshot 2026-07-01 164207" src="https://github.com/user-attachments/assets/9bf7e1e6-15b6-4f61-802a-5d58051fce83" />
 |
| Home |<img width="1911" height="948" alt="Screenshot 2026-07-01 171309" src="https://github.com/user-attachments/assets/68763d79-552f-4440-b6a9-a3a2693d764c" />
  |
| Dashboard |<img width="1913" height="942" alt="Screenshot 2026-07-01 164342" src="https://github.com/user-attachments/assets/5ffa19f1-c5c8-4a59-80df-fe2c77c189eb" />
|

| Report | <img width="1917" height="935" alt="Screenshot 2026-07-01 164442" src="https://github.com/user-attachments/assets/6bc5d696-83e2-4180-8bf4-061d78ada397" />
 |
| Students | <img width="1909" height="943" alt="Screenshot 2026-07-01 164521" src="https://github.com/user-attachments/assets/bb5eac3b-23f9-42da-840f-8f5aa8c0d5e0" />
 |
| About |<img width="1916" height="926" alt="Screenshot 2026-07-01 164306" src="https://github.com/user-attachments/assets/b2c58a32-7202-44d8-b4cb-9298cd3863da" />
  |
| Contact | <img width="1912" height="949" alt="Screenshot 2026-07-01 164543" src="https://github.com/user-attachments/assets/76c445e1-6510-40fd-8d16-bf1ec8f8f7e8" />
 |

---

## 📝 What I Learned

- Structuring a multi-page HTML project
- CSS Flexbox and Grid for responsive layouts
- JavaScript form validation and DOM manipulation
- Session-based authentication using sessionStorage
- Animated counters and progress bars with JavaScript
- Real-time search and filter logic
- Mobile-first responsive design techniques
- Professional UI/UX design principles
- Git version control and GitHub project hosting

---

## 📝 Notes

- Front-end prototype only — no backend or database connected
- All student data is hardcoded for demonstration
- Dynamic backend will be added in upcoming project phases

---

## 👤 Author

| Field | Details |
|-------|---------|
| *Name* | Zeeshan Haider |
| *Institution* | Abasyn University Islamabad Campus |
| *Internship* | Web Development Internship — Week 2 @codioro House (Private) Limited|
| *Project* | EduTrack Student Performance Analytics Portal |
| *Year* | 2026 |

---

This project was built for educational and internship purposes.
© 2026 EduTrack Analytics Portal
