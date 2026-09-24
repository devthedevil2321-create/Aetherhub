# 🪐 AetherHub v1.0

A secure, terminal-style web dashboard designed to embed learning portals, track batch milestones, and provide direct developer communication.

## 🚀 Key Features

*   **Secure Gatekeeper:** Blocks access with a 4-digit security PIN lock screen to ensure environment integrity.
*   **Persistent Batch Progress Dashboard:** An interactive progress tracker (\(0\%\) to \(100\%\)) that automatically saves milestones to the browser's local storage.
*   **Seamless Embedded Workspace:** Uses an integrated `<iframe>` viewport to load external platforms directly inside the terminal layout without forcing external redirects.
*   **Quick-Chat Connection Node:** A floating, animated communication node linking users directly to WhatsApp for rapid support.

---

## 🛠️ Configuration

Open `src/app/page.tsx` (or your component file) and update the **Configuration Constants** at the top of the file:

```tsx
// Configuration Constants
const SECRET_PIN = '1234';           // Set your private 4-digit access code
const WHATSAPP_NUMBER = '911234567890'; // Your number with country code (no '+' or spaces)
const PORTAL_URL = 'https://studypanda.live'; // The platform you want to embed
```

---

## 💻 Tech Stack & Deployment

*   **Framework:** Next.js (App Router with `'use client'`)
*   **Library:** React (Hooks: `useState`, `useEffect`)
*   **Styling:** Tailwind CSS (featuring dark mode utility classes, custom transitions, and pulse animations)
*   **Icons:** Inline optimized SVG vectors

### Getting Started

1. Clone or copy the component into your Next.js project.
2. Ensure Tailwind CSS is configured in your project.
3. Run the development server:
   ```bash
   npm run dev
   ```

---

## ⚠️ Cross-Origin Embed Note
This platform renders workloads inside a standard viewport frame. Ensure that your target `PORTAL_URL` does not explicitly reject embedding via `X-Frame-Options` or `Content-Security-Policy (CSP)` server headers.

---

## ⚡ Credits

Made with ❤️ by **Dev Aradhya Swain**
# Aetherhub