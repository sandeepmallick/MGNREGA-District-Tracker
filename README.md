# 🌾 MGNREGA District Performance Tracker

An interactive web dashboard built to help citizens of India, especially those from rural areas, easily understand their district’s performance under the MGNREGA (Mahatma Gandhi National Rural Employment Guarantee Act) program.

This project uses the official MGNREGS Open API from data.gov.in
 and presents complex government data in a simple, visual, and accessible format for low-literacy users.

# 🧭 Project Overview

The Government of India releases monthly data about MGNREGA district-level performance via open APIs.
However, these datasets are not easily usable by ordinary citizens due to:

Low data literacy

Technical complexity of APIs

Inconsistent uptime and throttling by the API provider

To address this, this project visualizes the key employment and financial metrics in an easy-to-understand, mobile-friendly, and language-localized interface.

# ✨ Features-Interactive Dashboard

Displays total workers, projects, average wages, and employment days per household

Visual charts show 6-month performance trends for better understanding

# 🌍 State & District Selector

Users can select their State and District to view localized MGNREGA performance data

# 📊 Visual Trends

Line and bar charts showing workers employed, projects taken up, and fund utilization trends

# 🌐 Multilingual Support

Built-in language selector (supports English + Regional Languages) for accessibility

# 🧠 Low-Literacy Friendly Design

Use of icons, colors, and visuals instead of complex text

Simple numeric and symbolic representations (e.g., ₹ for wages, 👷‍♂️ for workers)

Consistent layout and large readable fonts

# ⚡ Offline Data Caching (Production Ready)

Uses a server-side cache to store API responses

Automatically refreshes data every 24 hours to prevent API downtime or rate-limit issues

Ensures that the website remains available even when the API is down

# 📱 Mobile-Friendly UI

Responsive design optimized for both smartphones and desktop users

# 🏗️ System Architecture
                ┌────────────────────────┐
                │  User (Web/Mobile)     │
                └────────────┬───────────┘
                             │
                             ▼
               ┌──────────────────────────┐
               │   React Frontend (Vercel)│
               │  - Charts, UI, Language   │
               └────────────┬─────────────┘
                             │
                             ▼
             ┌────────────────────────────────┐
             │ Node.js Server (Express)        │
             │ - Fetches data from MGNREGS API │
             │ - Caches responses (24h)        │
             │ - Returns JSON to frontend      │
             └────────────────────────────────┘
                             │
                             ▼
             ┌────────────────────────────────┐
             │ MGNREGS Open API (data.gov.in)  │
             └────────────────────────────────┘


# 📦 Installation & Setup
# 1️⃣ Clone the Repository
bash

Copy code

git clone https://github.com/yourusername/mgnrega-district-tracker.git

cd mgnrega-district-tracker

# 2️⃣ Install Dependencies
bash

Copy code

npm install

# 3️⃣ Add Your API Key
Create a .env file in the root folder:

ini
Copy code

MGNREGA_API_KEY=579b464db66ec23bdd000001f9974a78b0124f856dcb93c1fcb2f4df

# 4️⃣ Run the Development Server
bash
Copy code
npm run dev
5️⃣ Open in Browser
Visit: http://localhost:3000

# 🧪 Example Data Visualized
Metrics Displayed:

Total Workers Employed: e.g., 32.1K people employed

Total Projects Taken Up: 23,771

Average Wage: ₹275/day/person

Average Days/Household: 21

Visuals include:

Workers Trend (Last 6 Months)

Works Taken Up Trend (Last 6 Months)

Comparative analysis vs last month

# 🧩 Design Philosophy
The interface is designed for citizens with minimal digital literacy:

Clear color-coded cards

Use of icons for each metric

Local language labels (for e.g., Hindi, Telugu, Odia)

Minimal text, maximum visuals

# 🌏 Scalability & Production Readiness
API Caching Layer to reduce dependency on live API uptime

Scheduled auto-refresh (every 24 hours)

Stateless frontend hosting for easy scaling

CDN delivery (via Vercel) for fast load times across India

# 🧑‍💻 Developer
Author: Sandeep mallick
Year: 2025
Project Type: Academic / Social Welfare Data Visualization
Live Demo: mgnrega-district-tracker.vercel.app

# 📜 License
This project is released under the MIT License.


🖼️ Preview
https://github.com/sandeepmallick/MGNREGA-District-Tracker/issues/1#issue-3561835031

