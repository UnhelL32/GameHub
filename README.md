Backlog Vault: Video Game Collection Tracker
A modern, responsive, zero-setup React application designed to help you track your playthroughs of 80 of the most defining video games across RPG, FPS, Third-Person, and RTS genres.
The entire application runs from a single index.html file, requiring no build tools, no backend server, and no installation.
Features
 * Zero-Setup Execution: Runs entirely in the browser. Just double-click the file to start.
 * Persistent Local Storage: Your progress (games played, start dates, and end dates) is automatically saved to your browser's local storage. You won't lose your data when you refresh or close the tab.
 * High-Quality Cover Art: Displays official, high-resolution box art sourced directly from Steam's Content Delivery Network and Wikimedia. (Hardcoded to bypass browser CORS restrictions).
 * Advanced Filtering & Search: Instantly filter your backlog by genre (RPG, FPS, Third-Person, RTS), completion status (Played/Unplayed), or search by title and developer.
 * Progress Tracking: Visual progress bar tracking your completion percentage against the 80-game database.
 * Responsive UI: Built with Tailwind CSS to ensure a seamless, app-like experience on desktop monitors, tablets, and smartphones.
Tech Stack
 * React 18: Loaded via CDN for state management and component rendering.
 * Tailwind CSS: Loaded via CDN for rapid, modern, dark-mode UI styling.
 * Babel (Standalone): Compiles JSX directly in the browser.
 * HTML5/JS: Native browser APIs for localStorage and IntersectionObserver.
How to Run
 * Create a new folder on your computer.
 * Save the provided code block as a file named index.html.
 * Double-click index.html to open it in your preferred web browser (Chrome, Firefox, Safari, Edge).
 * Start tracking your games!
Data Sources
The application includes a curated database of 80 critically acclaimed video games. Cover art is hotlinked directly from official sources to ensure fast loading and high resolution:
 * Steam Store CDN: Used for PC and multi-platform titles.
 * Wikimedia Commons: Used for console exclusives and classic titles (e.g., Nintendo, early PlayStation exclusives).
Modifying the Database
If you wish to add your own games to the tracker, open index.html in a text editor and locate the gamesDB array near the top of the <script type="text/babel"> tag.
You can add a new game by following the established JSON structure:
{ 
  "id": 81, 
  "title": "Your Game Title", 
  "genre": "RPG", 
  "platform": "PC", 
  "developer": "Developer Name", 
  "cover": "https://link-to-image.jpg" 
}
