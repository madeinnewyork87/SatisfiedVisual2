Satisfied Visual Planner 🏭✨
A powerful, visual, node-based logistics calculator and factory planner for the game Satisfactory.
Built entirely with vanilla web technologies (HTML, JS, Tailwind CSS), this planner allows you to drag, drop, wire, and mathematically perfect your production lines. It also features a cutting-edge AI Architect powered by Google Gemini to instantly generate complex factory layouts from simple text prompts.
🌟 Key Features
🧠 AI Architect: Describe your end-game goal (e.g., "10 Heavy Modular Frames per minute"), and the AI will automatically spawn, configure, and wire the necessary machines on your canvas.
⚖️ Auto-Balance & Auto-Arrange: Instantly recalculate exact clock speeds across your entire production chain to match your target output. Cleans up messy layouts into perfectly aligned, layered trees.
🔌 Visual Node Wiring: Connect machine outputs to inputs visually. Lines automatically turn red if there is an input deficit.
🏗️ Auto-Build: Click on an unsatisfied input to automatically spawn and wire the required upstream machines.
⚙️ Advanced Game Mechanics: Full native support for Overclocking (up to 250%), Somersloops, Alternate Recipes, and SAM resources.
📊 Factory Ledger: Real-time calculation of net power consumption and raw resource extraction demands.
💾 Import / Export Blueprints: Save your intricate factory designs as JSON files to share with the community or back up your work.
🛠️ Custom Recipes: Load your own custom recipes.js files to support game mods or custom balance tweaks.
🚀 Getting Started
Because the planner is built with vanilla HTML, JavaScript, and Tailwind CSS (via CDN), there are no complex build steps, npm installs, or local servers required.
Option 1: Live Web Version
Just visit the live GitHub Pages link:
👉 Play with the Planner Here (Update link if different)
Option 2: Run Locally
Clone or download this repository.
Open planner.html in any modern web browser.
Note: For the best experience and to avoid strict local CORS policies with external scripts, it is recommended to serve the folder via a simple local web server (e.g., VS Code Live Server).
🤖 Setting Up the AI Architect (Gemini API)
To use the AI Architect feature locally or on the live web version, you will need a free Google Gemini API key.
Go to Google AI Studio and create a free API Key.
Open the Satisfied Visual Planner.
Open the Config & Alts tab on the left sidebar.
Under API Settings, paste your key and click Save API Key.
Your key is saved securely in your browser's local storage and is never sent anywhere except directly to Google's API.
🎮 Controls & Usage
Add Machines: Open the Library tab on the left, search for an item, and drag it onto the canvas.
Connect Machines: Click and drag from a green output node to an orange input node.
Pan: Middle-mouse click & drag, or Shift + Left-click & drag.
Zoom: Scroll wheel.
Select Multiple: Left-click and drag a selection box, or hold Ctrl/Shift and click specific cards.
Context Menu: Right-click any machine card to Duplicate, Lock, Sync, Auto-Balance, or Auto-Build.
Edit Rates: Click directly on any number (Buildings, Clock Speed, Somersloops, or Input/Output rates) to type a new value, or use the pop-up slider.
🔧 Architecture / Tech Stack
HTML5 Canvas Alternative: Uses absolute DOM positioning and SVG paths (#connector-svg) for rendering lines, making elements highly interactive and stylable with CSS.
Tailwind CSS: Handled via CDN for rapid, highly-responsive UI styling.
Vanilla JavaScript (ES6): No React, Vue, or Angular. State is managed centrally in a single state object.
Gemini 1.5 Flash: Utilizes the @google/gemini-2.5-flash endpoint with strict JSON schema enforcement to parse natural language into structured graph topologies.
🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request
☕ Support
If this tool helped you organize your spaghetti factory into a beautifully efficient machine, consider supporting the project!
📜 License
Distributed under the MIT License. See LICENSE for more information.
