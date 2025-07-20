Event Calendar
A dynamic, interactive event calendar built with React, Vite, and Tailwind CSS. This application allows users to manage their schedule with features like adding, editing, deleting events, recurring events, and drag-and-drop functionality.

Features
📅 Monthly Calendar View - Traditional calendar layout with navigation
➕ Event Management - Add, edit, and delete events
🔄 Recurring Events - Support for daily, weekly, and monthly recurrence
🎯 Drag & Drop - Reschedule events by dragging them to different dates
🔍 Search & Filter - Find events by title/description and filter by category
⚠️ Conflict Detection - Prevents overlapping events at the same time
💾 Local Storage - Events persist across browser sessions
🎨 Color Categories - Visual organization with color-coded categories
📱 Responsive Design - Works on desktop and mobile devices
Installation
Create a new directory and navigate to it:
bash
mkdir event-calendar
cd event-calendar
Initialize the project:
bash
npm create vite@latest . --template react
Install dependencies:
bash
npm install
npm install date-fns react-dnd react-dnd-html5-backend
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
Copy all the provided files to their respective locations:
Copy package.json (replace the generated one)
Copy all files from the artifacts above to their specified paths
Make sure the folder structure matches:
event-calendar/
├── public/
├── src/
│   ├── components/
│   │   ├── Calendar.jsx
│   │   ├── CalendarDay.jsx
│   │   ├── EventItem.jsx
│   │   ├── EventModal.jsx
│   │   └── SearchFilter.jsx
│   ├── context/
│   │   └── EventContext.jsx
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── tailwind.config.js
├── postcss.config.js
└── vite.config.js
Start the development server:
bash
npm run dev
Open your browser and navigate to the URL shown in the terminal (usually http://localhost:5173)
Usage
Adding Events
Click the "Add Event" button or click on any calendar day
Fill in the event details (title, date, time, description, category)
Choose recurrence options if needed
Click "Add Event"
Editing Events
Click on any event in the calendar
Modify the details in the modal
Click "Update Event"
Deleting Events
Click on an event to open the edit modal
Click "Delete Event"
Confirm the deletion
Drag and Drop
Simply drag any event to a different day to reschedule it
The calendar will highlight valid drop zones
Search and Filter
Use the search bar to find events by title or description
Use the category dropdown to filter events by type
Combine both for precise filtering
Project Structure
src/components/ - React components
Calendar.jsx - Main calendar grid and navigation
CalendarDay.jsx - Individual day cell with drag-drop support
EventItem.jsx - Event display component with drag functionality
EventModal.jsx - Form for adding/editing events
SearchFilter.jsx - Search and filter controls
src/context/ - State management
EventContext.jsx - Global event state and operations
Technologies Used
React 18 - UI framework
Vite - Build tool and development server
Tailwind CSS - Utility-first CSS framework
date-fns - Date manipulation library
react-dnd - Drag and drop functionality
Local Storage - Data persistence
Browser Support
This application works in all modern browsers that support:

ES6+ JavaScript features
CSS Grid and Flexbox
HTML5 Local Storage
HTML5 Drag and Drop API
Contributing
Feel free to submit issues and enhancement requests!

License
This project is open source and available under the MIT License.

