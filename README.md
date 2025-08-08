Repository Structure & Files
The project includes the following key files and folders:

index.html, about.html, chatbot.html, contact.html, feedback.html, live-news.html, statistics.html, vaccine.html, nearby-camps.html, and chennai_disease_tracker.html — forming a multi-page static frontend.

app.py — a Python backend entry point (likely using Flask or similar).

style.css for styling.

Media assets: vid.mp4, vid1.mp4, vid2.mp4, and images (pic1.jpg, etc.).

Insights:
The HTML files suggest a full interface with multiple sections such as surveys, chat features, nearby camps, news, vaccine info, and disease tracking.

chennai_disease_tracker.html is the page where disease trend charts are implemented.

app.py likely handles routing or API-like backend functionality.

statistics.html includes charts and map features as we previously integrated.

Features Implemented Aligned with the Hackathon Requirements
Core Features:
** Anonymized vaccination tracking** – The site allows data display but actual data collection from users or healthcare records would require backend support such as app.py.

** Visualization of Coverage** – statistics.html shows bar charts, pie charts, and a heatmap for vaccination zones using Chart.js and Leaflet, aligned with tracking coverage by location.

** Disease & Outbreak Monitoring** – In chennai_disease_tracker.html, disease cases today and monthly trends are visualized with charts, and outbreak risk is detected based on month-over-month increases.

Bonus Capabilities:
** Outbreak Risk Simulation** – Monthly trend comparison with thresholds flag risky outbreaks—fulfills bonus requirement.

** Chatbot** – There’s chatbot.html, showing an interactive chatbot component (possibly simulated).

** Nearby Camps Display** – nearby-camps.html suggests location-service-like features (possibly interfacing with maps or geolocation).

Summary Table
Feature	Status	Description
Data Collection	Partial	UI in place, backend may need to integrate actual data submission
Coverage Visualization		Bar chart, pie chart, heatmap implemented
Reminders for Vaccines		Not directly visible — potential to integrate
Outbreak Risk Detection		Done in disease tracker page
Government API Integration		Not present yet
Chatbot		Present but static UI; needs intelligence
Nearby Vaccination Camps		UI exists; backend functionality pending

🧠 Overview
You have a multi-page HTML/CSS/JS frontend with some Python backend (app.py). Likely intended to be run locally as a static site or with Flask.

✅ Step-by-Step Instructions
🔁 1. Clone the GitHub Repository
Open Terminal (Mac/Linux) or CMD/PowerShell (Windows), and run:

bash
Copy
Edit
git clone https://github.com/sexyna/Vaccitrack.git
cd Vaccitrack
🌐 2. Open the Website in Your Browser (HTML Only)
You can test the static part without Python.

Option A: Just Open index.html
Open the project folder.

Double-click index.html or right-click → “Open with” → your browser.

✅ You’ll see the homepage with the background video, logo, and navigation.

But some features (like chatbot logic, live API, or data submission) may not work without running the backend.

⚙️ 3. Run Backend Locally (if using app.py)
If app.py is using Flask, follow these steps:

📦 Install Python Dependencies
Make sure you have Python 3 installed.

Then in the project folder, run:

bash
Copy
Edit
pip install flask
▶️ Run the Server
bash
Copy
Edit
python app.py
Then open this in your browser:

cpp
Copy
Edit
http://127.0.0.1:5000
✅ You should now see the site being served locally with backend capabilities.

🗺️ 4. Test Features
Navigate to these pages:

Page	File	Description
Home	index.html	Landing page with video and links
Vaccination Stats	statistics.html	Charts + heatmap of zones
Disease Tracker	chennai_disease_tracker.html	Trend line chart & outbreak risk detection
Chatbot	chatbot.html	UI for simulated chat
Nearby Camps	nearby-camps.html	Map or location info for vaccine camps

💡 Optional: Serve HTML via Live Server (VS Code)
If you have VS Code installed:

Install the Live Server extension.

Open project in VS Code.

Right-click index.html → "Open with Live Server".

✅ Auto-refresh, and no browser security issues for local JS.

🛠 Common Issues & Fixes
Problem	Fix
JS charts not loading	Ensure Chart.js is connected (via CDN or locally)
Map not loading	Ensure internet access (Leaflet loads tiles from web)
Background video missing	Ensure vid.mp4 is in the root directory
CORS errors	Use Live Server or Python Flask to serve locally
