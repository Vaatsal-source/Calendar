🌌 Cosmic Calendar
A highly immersive, interactive, and visually stunning calendar component built with Next.js, Framer Motion, and Tailwind CSS. This calendar doesn't just manage dates; it provides a "cosmic" experience with dynamic backgrounds, smooth animations, and local persistence.

✨ Features
Interactive Date Selection: Single-click to select a start date and a second click to select an end date to define a range.

Dynamic Visuals:

Cosmic Background: A month-aware dynamic background that changes its visual theme based on the selected month.

Hero Imagery: The side panel updates with thematic images for each month.

Cursor Glow: A fixed glow follows your mouse movement for a depth-parallax effect (desktop only).

Custom Holidays: Double-click any day to open a sleek modal and mark it as a custom holiday.

Persistent Notes: Jot down thoughts or plans for specific date ranges. Your notes are automatically saved to your browser's localStorage.

Ultra-Smooth Animations: Powered by Framer Motion for layout transitions, month switching (slide effects), and hover interactions.

Responsive Design: Fully optimized for mobile, tablet, and desktop views.

🛠️ Tech Stack
Framework: Next.js (App Router)

Styling: Tailwind CSS

Animations: Framer Motion

Components: Dynamic imports for client-side heavy visuals.

🚀 Getting Started
1. Prerequisites
Ensure you have the following components/files in your project structure:

CosmicBackground.js: The visual engine for the background.

images.js: An array or object exporting the HERO_IMAGES paths.

2. Installation
Install the necessary dependencies:

Bash
npm install framer-motion lucide-react
# or
yarn add framer-motion lucide-react
3. Usage
Simply place the Page.jsx into your Next.js app directory. Ensure your tailwind.config.js is set up to handle the dark mode and custom opacity colors used in the code.

📂 Key Logic Overview
Date Range Logic: The handleDateClick function intelligently toggles between selecting a start date, updating the range, or resetting selections.

Local Storage Sync: Two useEffect hooks monitor customHolidays and notesMap to ensure your data persists across page refreshes without a backend.

AnimatePresence: Used for the month headings and calendar grids to provide a sliding "carousel" feel when navigating through time.

🎨 Customization
You can easily change the aesthetic by modifying the :root variables or the Tailwind classes:

Glow Color: Change bg-blue-500/20 in the cursor glow div.

Accent Gradient: Modify the accentStyle object in the calendar grid (currently a purple-to-orange gradient).

📝 License
This project is open-source. Feel free to use and modify it for your own personal or commercial projects.

Built with ✨ and ⚛️ by Vaatsalya Srivastava
