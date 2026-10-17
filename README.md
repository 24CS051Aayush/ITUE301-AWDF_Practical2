# ITUE301 - Advanced Web Development Frameworks
## Practical 2: State Management and Routing in React

### Student Details
- **Student ID:** 24CS051
- **Student Name:** Aayush Malhotra
- **Subject Code & Name:** CSE304 / ITUE301: Advanced Web Development Frameworks
- **Department:** Department of Computer Science and Engineering
- **Institution:** Chandubhai S Patel Institute of Technology (CSPIT), CHARUSAT
- **Academic Year:** 2025-26

---

### Aim
To implement reactive state management using `useState` and multi-page single-page application (SPA) navigation using `React Router v6` in the existing student portfolio project.

---

### Application Architecture & Routes
```text
App.jsx (wrapped in <BrowserRouter> inside main.jsx)
 ├── NavBar.jsx         (Links to all routes using <NavLink>, dark/light mode toggle)
 ├── Route: "/"         → Home.jsx (composes Header, Overview toggle, About, Skills)
 ├── Route: "/projects" → Projects.jsx (lists connected full-stack coursework modules)
 ├── Route: "/contact"  → Contact.jsx (controlled form with useState, live preview & char count)
 └── Route: "*"         → NotFound.jsx (custom 404 page for unknown routes)
```

---

### Key Features Implemented
1. **Client-Side Routing with React Router v6**:
   - Integrated `<BrowserRouter>`, `<Routes>`, `<Route>`, and `<NavLink>`.
   - Prevents full-page browser reloads, providing seamless single-page application experience.
   - Distinct active route indicator on navigation items.
2. **Reactive State Management (`useState`)**:
   - **Form Input State**: Controlled component inputs for name, email, subject, and message.
   - **Real-Time Input Preview**: Live reflection of user typing without form submission.
   - **Live Character Counter**: Dynamic character counter tracking length and limits.
   - **UI Visibility Toggles**: Interactive help/guidelines tooltip and coursework overview toggle.
   - **Global Theme State**: Light / Dark mode toggle affecting root container.
3. **404 Not Found Handling**:
   - Wildcard catch-all route (`*`) rendering a custom `NotFound` error view with navigation back to Home.

---

### Getting Started

#### Prerequisites
- Node.js (v18+)
- npm (v9+)

#### Installation & Execution
```bash
# 1. Clone repository
git clone https://github.com/24CS051Aayush/ITUE301-AWDF_Practical2.git
cd ITUE301-AWDF_Practical2

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
```

App runs by default at `http://localhost:5173`.
