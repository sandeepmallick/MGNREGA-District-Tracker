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

# 🧰 Tech Stack
Layer	Technology
Frontend	React.js, Tailwind CSS, Recharts
Backend	Node.js (Express), Axios
API Source	MGNREGS Open API – data.gov.in

Hosting	Vercel (Frontend), Optional Backend on Render/Express
Caching	JSON file cache / server memory store
