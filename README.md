# 📦 RentRax - Rental Site Web Technology Project

An interactive, responsive multi-page web application for an equipment and goods rental platform featuring the official **RentRax** brand identity. Designed strictly according to the academic wireframe specification (**Course Code: 01CE1306 – Web Technology Project**, Marwadi University).

---

## 🌟 Quick Overview

* **Brand & Platform:** RentRax (*"Rentals for Everything"*)
* **Tagline:** *"Rent anything you want, anytime you want."*
* **Project Architecture:** Clean 3-Tier Folder Separation (`client/`, `admin/`, `about/`)
* **Company Logo:** [`logo.png`](./logo.png) integrated across headers, navigation sidebars, and authentication screens.
* **Design Specification:** [`Rental_Site_Wireframe_Final_Format.pdf`](./Rental_Site_Wireframe_Final_Format.pdf) (12 Wireframe Pages)
* **Technologies Used:** HTML5, Tailwind CSS, Bootstrap 5.3.8, Bootstrap Icons (WebFont), Vanilla JavaScript (with DOM form validation), CSS3
* **Graphics & Media:** Free high-resolution online photography (Unsplash CDN) and font-based icons (Zero SVGs in markup)

---

## 🚀 How to Run the Project

No build step, Node.js, or backend installation is required.

1. **Root Multi-Portal Entry:**
   * Open [`index.html`](./index.html) in any modern browser to access the central portal hub.
2. **Direct Module Access:**
   * **Client Portal:** Open [`client/login.html`](./client/login.html) or [`client/dashboard.html`](./client/dashboard.html).
   * **Admin Portal:** Open [`admin/login.html`](./admin/login.html) or [`admin/dashboard.html`](./admin/dashboard.html).
   * **About Platform:** Open [`about/index.html`](./about/index.html).
3. **VS Code Live Server (Optional):**
   * Right-click [`index.html`](./index.html) and select **"Open with Live Server"**.

---

## 📂 Project Directory Structure

The project is structured into **3 dedicated folders** (`client/`, `admin/`, `about/`), with shared assets at the root and zero duplicate files:

```
wt project/
├── 🌐 Root Entry & Shared Assets
│   ├── index.html                           # Central Portal Hub (Client, Admin, About)
│   ├── shared-shell.css                     # Unified Glassmorphic shell, topbar & responsive sidebar
│   ├── logo.png                             # Official RentRax brand emblem
│   ├── 2516264.webp                         # Ambient backdrop texture
│   ├── README.md                            # Comprehensive project manual
│   └── Rental_Site_Wireframe_Final_Format.pdf # Original wireframe blueprint
│
├── 👤 client/ (User Portal - Fig. 1.1 - 1.7)
│   ├── login.html                           # Fig 1.1: Sign In & Registration Modal with JS Validation
│   ├── dashboard.html                       # Fig 1.2: Metrics & Rented Items Overview
│   ├── profile.html                         # Fig 1.3: User Profile & Avatar Preview Upload
│   ├── order-history.html                   # Fig 1.4: Rental History with Tabs & Live Search
│   ├── rewards.html                         # Fig 1.5: Loyalty Points, Credits & Payment Ledger
│   ├── items.html                           # Fig 1.6: Product Catalog with Live Filter & Search
│   └── rent-request.html                    # Fig 1.7: Rental Checkout with Dynamic Days/Price Math
│
├── 🛡️ admin/ (Management Portal - Fig. 2.1 - 2.5)
│   ├── login.html                           # Fig 2.1: Admin Authentication with Security Badge
│   ├── dashboard.html                       # Fig 2.2: Management KPIs & Recent Requests Summary
│   ├── daily-records.html                   # Fig 2.3: Daily Issued & Returned Logs with Date Picker
│   ├── rent-requests.html                   # Fig 2.4: Approval Desk with Approve/Reject/View Modals
│   └── users-list.html                      # Fig 2.5: User Directory with Live Search & Profile View
│
└── ℹ️ about/ (Platform & Documentation)
    └── index.html                           # Comprehensive Platform Story, Features, Architecture & Credits
```

---

## 📑 Pages & Wireframe Mapping Directory

### 👤 1. Client-Side Pages (`client/`)

| Wireframe # | Page Description | File Path | Key Features |
| :--- | :--- | :--- | :--- |
| **Fig. 1.1** | **User Login** | [`client/login.html`](./client/login.html) | Brand hero banner, login card, form validation, "Remember me", Sign-Up modal, links to Admin and About portals. |
| **Fig. 1.2** | **User Dashboard** | [`client/dashboard.html`](./client/dashboard.html) | 4 Summary metric cards, recent rented items with expandable details, active rentals summary. |
| **Fig. 1.3** | **Profile Page** | [`client/profile.html`](./client/profile.html) | User portrait photo with client-side preview upload, editable profile fields, update confirmation feedback. |
| **Fig. 1.4** | **Order / Rent History** | [`client/order-history.html`](./client/order-history.html) | Filter tags (All, Returned, Ongoing), live table search, status badges (`Returned`, `Ongoing`, `Pending`). |
| **Fig. 1.5** | **Rewards & Payments** | [`client/rewards.html`](./client/rewards.html) | Reward Points card, Available Balance card, and past payment transactions receipt table. |
| **Fig. 1.6** | **Items for Rent** | [`client/items.html`](./client/items.html) | Instant category filters (All, Electronics, Furniture, Sports, Tools), live keyword search, item cards with free online photos, **"Rent Now"** buttons. |
| **Fig. 1.7** | **Rent Request / Checkout** | [`client/rent-request.html`](./client/rent-request.html) | Back navigation, dynamic product image & pricing, quantity stepper (`-` / `+`), interactive date pickers with automatic day & total calculations, and order confirmation modal. |

---

### 🛡️ 2. Admin-Side Pages (`admin/`)

| Wireframe # | Page Description | File Path | Key Features |
| :--- | :--- | :--- | :--- |
| **Fig. 2.1** | **Admin Login** | [`admin/login.html`](./admin/login.html) | Dedicated secure portal login, pre-filled demo admin credentials, direct switch to User login and About. |
| **Fig. 2.2** | **Admin Dashboard** | [`admin/dashboard.html`](./admin/dashboard.html) | High-level metrics (Total Users: 25, Total Items: 50, Total Requests: 12, Revenue: $320), recent rent requests table with status badges. |
| **Fig. 2.3** | **Daily Records** | [`admin/daily-records.html`](./admin/daily-records.html) | Date-picker filter bar, **"Items Issued Today"** log, and **"Items Returned Today"** log. |
| **Fig. 2.4** | **Rent Item Requests** | [`admin/rent-requests.html`](./admin/rent-requests.html) | Comprehensive request queue with live interactive `[Approve]` and `[Reject]` actions, plus detailed inspection modal `[View]`. |
| **Fig. 2.5** | **Users Directory** | [`admin/users-list.html`](./admin/users-list.html) | Registered members directory with portrait avatars, real-time search filter, and individual user profile modal. |

---

### ℹ️ 3. About & Information (`about/`)

| Wireframe # | Page Description | File Path | Key Features |
| :--- | :--- | :--- | :--- |
| **Platform Guide** | **About RentRax** | [`about/index.html`](./about/index.html) | Platform mission, 3-step rental journey, architecture guide, technology stack details, and portal cross-links. |

---

## 💡 Key Highlights & Enhancements

1. **Modular 3-Folder Structure:**
   * Cleanly separated into `client/` for renter screens, `admin/` for back-office management, and `about/` for documentation.
   * Duplicate files (`login2.html` and `2516264 (1).webp`) eliminated.
2. **Zero SVGs in Markup:**
   * Replaced inline SVG code with lightweight Bootstrap Icons font glyphs and free Unsplash high-resolution images.
3. **Official RentRax Branding:**
   * Consistent use of official logo (`logo.png`) and purple accent theme (`#7C3AED`) across every screen and shared stylesheet (`shared-shell.css`).
4. **Client-Side Form & Workflow Validation:**
   * Real-time JavaScript validation on login, registration, checkout date calculation, and profile editing.
5. **Interactive Controls:**
   * Instant search filtering on catalog, order history, and user directories without page reloading.
   * Live approval/rejection state transitions in admin request desks.
6. **Fully Responsive:**
   * Mobile slide-over navigation sidebar via `#menu-toggle`, flex/grid layouts, and glassmorphic card containers.

---

## 🔑 Demo Credentials

| Role | Username | Password | Direct Login Link |
| :--- | :--- | :--- | :--- |
| **Client / User** | `User` | `password123` | [`client/login.html`](./client/login.html) |
| **Administrator** | `admin` | `admin123` | [`admin/login.html`](./admin/login.html) |

---

## 👥 Academic Credits & Acknowledgements

* **Course Code:** 01CE1306 – Web Technology Project
* **Institution:** Faculty of Technology, Marwadi University, Rajkot
* **Project Theme:** RentRax - Multi-tier Online Rental Platform
* **Specification Source:** [`Rental_Site_Wireframe_Final_Format.pdf`](./Rental_Site_Wireframe_Final_Format.pdf)
