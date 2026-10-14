# 🚛 FreightShorts 
**FreightShorts** is Progressive Web App (PWA) built for trucking, middle-mile, and supply chain executives. It aggregates real-time industry news into a fast, Inshorts-style vertical card deck, interleaves a 3-tier Freight Domain Academy, includes a hands-free Podcast mode, and uses **Google Gemini AI** for live quantitative synthesis and contextual Q&A. 

A very early version - powered by Gemini.

---

## ✨ Core Features

| Feature | Description |
| :--- | :--- |
| ** Live Multi-Source Feeds** | Aggregates and deduplicates live RSS streams from *FreightWaves*, *Transport Topics*, *Overdrive*, *Supply Chain Dive*, and *On The Seams*. |
| ** Auto-Classifier** | Automatically routes incoming stories into **Fraud & Safety**, **Cost & Capacity**, **Regulations & Compliance**, and **AI & Tech Innovation**. |
| ** 3-Tier Domain Academy** | Injects an educational masterclass slide every 4th card. Switch complexity on the fly between **Tier 201 (Ops & Unit Economics)**, **Tier 301 (Quant & Legal)**, and **Tier 401 (Network Topology)**. |
| ** Level 2 Executive Brief** | Slide-up iOS bottom sheet displaying 3 extracted KPI metrics, quantitative formulas, and a 3-part breakdown (*Underlying Mechanics*, *Second-Order Network Effects*, and *Actionable Playbook*). |
| ** Ask Gemini Co-Pilot** | Card-scoped AI chat inside the bottom sheet with one-tap executive prompts to stress-test unit economics, routing guides, and risk exposure. |
| ** Hands-Free Podcast Mode** | Native neural text-to-speech engine that reads the feed aloud and automatically advances through the card deck while commuting. |

---

## 📲 Step 1: Install as a Full-Screen App on Your Phone (2 Minutes)

### **On iPhone (iOS Safari)**
> [!IMPORTANT]
> You must use **Safari** on iOS to install full-screen Home Screen web apps.

1. Open the hosted `https://` app link in **Safari** on your iPhone.
2. Tap the **Share** button at the bottom center of the screen (the square with the upward arrow `↑`).
3. Scroll down the share menu and tap **Add to Home Screen**.
4. Confirm the name **FreightShorts** and tap **Add** in the top-right corner.
5. **Launch from Home Screen:** Close Safari and tap the new **FreightShorts** icon on your Home Screen to open the app in standalone full-screen mode.

### **On Android (Chrome)**
1. Open the hosted `https://` app link in **Chrome**.
2. Tap the **Three Dots (`⋮`)** menu in the top-right corner.
3. Tap **Add to Home screen** or **Install app**.

---

## 🔑 Step 2: Enable Free Google Gemini AI Features (60 Seconds)

The live news feed, 3-tier Domain Academy, and Podcast audio work immediately out of the box. To unlock real-time **AI Synthesis (`✨ AI`)** and **Ask Gemini Q&A**, add a free Google Gemini API key:

1. Go to **[Google AI Studio (aistudio.google.com/apikey)](https://aistudio.google.com/apikey)** and sign in with a personal Gmail account.
2. Click **Create API key** -> **Create API key in new project**.
3. Copy the generated key string (supports both modern `AQ...` and `AIzaSy...` formats).
4. Open **FreightShorts** from your phone's Home Screen and tap **`⚙️ Key`** in the top-right header.
5. Paste your key into the box and tap **`Test & Auto-Discover Model`**.
   - *The app will query Google's `ListModels` endpoint, lock onto the newest active Flash model on your account, and display `✅ Connected`.*
6. Tap **`Save & Close`**.

> [!NOTE]
> **Privacy & Security:** Your API key is stored strictly inside your device's local browser storage (`localStorage`). It is never transmitted to or stored on the web hosting server. If you install the app on your iPhone Home Screen, make sure to paste your key **after** launching the app from the Home Screen icon.

---

## 🧭 Step 3: How to Use the App

* **Swipe Up / Down (or tap `↑ Prev` / `Next ↓`):** Flip through live 60-word executive summaries.
* **Filter by Pillar:** Tap the horizontal chips beneath the header (*Fraud & Safety*, *Cost & Capacity*, *Regulations*, *AI & Tech*, or *🎓 Academy*) to isolate specific topics.
* **Switch Academy Complexity (`🎓 Tier 201 / 301 / 401`):** Use the dropdown in the top header to adjust the technical and mathematical depth of the Domain Academy slides.
* **Open Level 2 Deep Dive (`✨ Level 2 & Ask AI`):** Tap the blue button in the bottom thumb dock to slide up the structured **Executive Brief**.
* **Chat with Gemini (`💬 Ask Gemini AI` Tab):** Inside the bottom sheet, switch to the **Ask Gemini AI** tab to tap a suggested prompt chip or type custom questions scoped to that exact article.
* **Live AI Rewrite (`✨ AI` in Top Header):** Tap **`✨ AI`** on any raw RSS news card to have Gemini dynamically synthesize a sharper 60-word thesis, extract 3 KPI pills, and build a quantitative formula for that story.
* **Listen Hands-Free (`🎧 Audio`):** Tap **`🎧 Audio`** in the bottom dock to start continuous podcast narration with auto-advance.

---

##  Hosting & Deployment
Because the entire application lives inside a single `index.html` file with zero build steps or backend dependencies, you can deploy it anywhere:

1. **GitHub Pages:** Commit `index.html` to the root of this repository -> go to **Settings** -> **Pages** -> select the **`main`** branch -> click **Save**.
2. **Netlify Drop:** Drag and drop the folder containing `index.html` onto **[app.netlify.com/drop](https://app.netlify.com/drop)**.
3. **Tiiny.host:** Drag and drop `index.html` onto **[tiiny.host](https://tiiny.host)** for an instant `https://` link.
