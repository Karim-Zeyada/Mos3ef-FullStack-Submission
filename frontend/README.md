# Mos3ef Frontend

**Mos3ef** is a modern, responsive web application built with **React 19** and **Vite**, designed to provide a seamless experience for patients and hospitals. It features a clean UI powered by **Tailwind CSS 4** and **shadcn/ui**.

## 🚀 Features

*   **Modern UI/UX:** Built with Tailwind CSS and shadcn/ui for accessible and beautiful components.
*   **Fast Performance:** Powered by Vite for lightning-fast development and building.
*   **Interactive Maps:** Integrated Leaflet maps for hospital location services.
*   **Responsive Design:** Fully optimized for desktop, tablet, and mobile devices.
*   **Secure Authentication:** JWT-based auth with role management (Patient/Hospital).
*   **Real-time Feedback:** Toast notifications and form validation using React Hook Form.

## 🛠 Tech Stack

*   **Framework:** [React 19](https://react.dev/)
*   **Build Tool:** [Vite](https://vitejs.dev/)
*   **Styling:** [Tailwind CSS 4](https://tailwindcss.com/)
*   **Routing:** [React Router DOM 7](https://reactrouter.com/)
*   **HTTP Client:** [Axios](https://axios-http.com/)
*   **Forms:** [React Hook Form](https://react-hook-form.com/)
*   **Icons:** [Lucide React](https://lucide.dev/)
*   **Maps:** [React Leaflet](https://react-leaflet.js.org/)
*   **UI Components:** [shadcn/ui](https://ui.shadcn.com/)

## 📂 Project Structure

```
src/
├── assets/          # Static assets (images, icons)
├── components/      # Reusable UI components
│   ├── ui/          # Base UI elements (Buttons, Inputs, Cards)
│   └── ...          # Feature-specific components (ServiceCard, NavBar)
├── Context/         # Global state management (Auth, Theme)
├── hooks/           # Custom React hooks
├── lib/             # Utility functions (cn, api helpers)
├── pages/           # Application pages (Auth, Home, Patient)
├── App.jsx          # Main application component
└── main.jsx         # Entry point
```

## ⚡ Getting Started

### Prerequisites
*   Node.js (v18 or higher)
*   npm or pnpm

### Installation

1.  **Navigate to the frontend directory:**
    ```bash
    cd frontend
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Start the development server:**
    ```bash
    npm run dev
    ```

4.  **Open your browser:**
    The app will be running at `http://localhost:5173` (or the port shown in your terminal).

## 📦 Scripts

*   `npm run dev`: Start the development server.
*   `npm run build`: Build the app for production.
*   `npm run preview`: Preview the production build locally.
*   `npm run lint`: Run ESLint to check for code quality issues.

## 🎨 UI Components
This project uses a component-first approach. Key components include:
*   **`ServiceCard`**: Displays service details with price, rating, and comparison options.
*   **`HospitalCard`**: Shows hospital information.
*   **`Map`**: Interactive map component for location selection.
*   **`NavBar` / `Header`**: Responsive navigation.

## 🤝 Contributing
1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.
