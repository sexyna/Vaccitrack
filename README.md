## Repository Structure & Files

The project includes the following key files and folders:

* `index.html`, `about.html`, `chatbot.html`, `contact.html`, `feedback.html`, `live-news.html`, `statistics.html`, `vaccine.html`, `nearby-camps.html`, and `chennai_disease_tracker.html` — forming a multi-page static frontend.
* `app.py` — a Python backend entry point (likely using Flask or similar).
* `style.css` for styling.
* Media assets: `vid.mp4`, `vid1.mp4`, `vid2.mp4`, and images (`pic1.jpg`, etc.).

### Insights:

* The HTML files suggest a full interface with multiple sections such as surveys, chat features, nearby camps, news, vaccine info, and disease tracking.
* `chennai_disease_tracker.html` is the page where disease trend charts are implemented.
* `app.py` likely handles routing or API-like backend functionality.
* `statistics.html` includes charts and map features as we previously integrated.

---

## Features Implemented Aligned with the Hackathon Requirements

### Core Features:

* **Anonymized vaccination tracking** – The site allows data display but actual data collection from users or healthcare records would require backend support such as `app.py`.
* **Visualization of Coverage** – `statistics.html` shows bar charts, pie charts, and a heatmap for vaccination zones using Chart.js and Leaflet, aligned with tracking coverage by location.
* **Disease & Outbreak Monitoring** – In `chennai_disease_tracker.html`, disease cases today and monthly trends are visualized with charts, and outbreak risk is detected based on month-over-month increases.

### Bonus Capabilities:

* **Outbreak Risk Simulation** – Monthly trend comparison with thresholds flag risky outbreaks—fulfills bonus requirement.
* **Chatbot** – There’s `chatbot.html`, showing an interactive chatbot component (possibly simulated).
* **Nearby Camps Display** – `nearby-camps.html` suggests location-service-like features (possibly interfacing with maps or geolocation).

---

## Summary Table

| Feature                    | Status  | Description                                                       |
| -------------------------- | ------- | ----------------------------------------------------------------- |
| Data Collection            | Partial | UI in place, backend may need to integrate actual data submission |
| Coverage Visualization     |         | Bar chart, pie chart, heatmap implemented                         |
| Reminders for Vaccines     |         | Not directly visible — potential to integrate                     |
| Outbreak Risk Detection    |         | Done in disease tracker page                                      |
| Government API Integration |         | Not present yet                                                   |
| Chatbot                    |         | Present but static UI; needs intelligence                         |
| Nearby Vaccination Camps   |         | UI exists; backend functionality pending                          |

---

### Next Steps I Can Assist With:

* Enhancing **data collection**—connecting forms to `app.py`.
* Adding **reminder system** (via email, push, SMS).
* Integrating **public health APIs**, such as official case counts.
* Improving **chatbot logic** or connecting to AI APIs.
* Enhancing the **nearby camps** feature with live geolocation or search.



## 🚀 Getting Started with VacciTrack

### 🧾 Overview

**VacciTrack** is a web-based platform designed to track and visualize vaccination status in communities. It was built as part of a hackathon challenge focused on public health awareness, data tracking, and outbreak risk detection.

---

### 📁 Clone the Repository

```bash
git clone https://github.com/sexyna/Vaccitrack.git
cd Vaccitrack
```

---

### 🌐 Run the Project (Frontend Only)

You can run the frontend directly by opening the HTML files:

1. Locate `index.html` in the project folder.
2. Right-click and choose **"Open with browser"** or simply double-click the file.

> ✅ This will launch the homepage of the site. Other pages like `statistics.html`, `vaccine.html`, and `chennai_disease_tracker.html` are also accessible the same way.

---

### ⚙️ Run with Backend (If using `app.py`)

If you want to enable backend features via Python (`app.py`):

#### 1. Install Dependencies

Make sure Python 3 is installed, then run:

```bash
pip install flask
```

#### 2. Start the Server

```bash
python app.py
```

Visit the app at:

```
http://127.0.0.1:5000
```

---

### 🧭 Navigation

| Page                | File                           | Description                             |
| ------------------- | ------------------------------ | --------------------------------------- |
| **Home**            | `index.html`                   | Landing page with intro and navigation  |
| **Statistics**      | `statistics.html`              | Vaccination stats, charts, and heatmap  |
| **Disease Tracker** | `chennai_disease_tracker.html` | Shows disease trends and outbreak risks |
| **Chatbot**         | `chatbot.html`                 | Simulated assistant for vaccine queries |
| **Nearby Camps**    | `nearby-camps.html`            | Displays nearby vaccination locations   |
| **Vaccine Info**    | `vaccine.html`                 | Vaccine eligibility and information     |
| **News**            | `live-news.html`               | Embedded live news section              |

---

### 📊 Key Features

* ✅ Anonymized vaccination tracking
* 📍 Location-wise coverage (bar, pie, and heatmap)
* 📈 Disease trend visualization
* ⚠️ Outbreak risk detection algorithm
* 🧠 Chatbot assistant (static logic)
* 🗺️ Nearby vaccination camps
* 🎥 Background video and interactive UI

---

### 💡 Bonus Implementation Ideas

* Government API integration for official case data
* Reminder system via SMS or email
* Real-time data submission and analytics
* Smarter AI-powered chatbot

---

### 🛠 Developer Notes

To enhance development:

* Use **VS Code Live Server** for easier local testing
* Ensure internet access for **Chart.js** and **Leaflet maps**
* Media assets like `vid.mp4` should be kept in the root directory

---

### 📬 Feedback & Contributions

We welcome improvements and feedback! Feel free to fork, contribute, or raise issues.
