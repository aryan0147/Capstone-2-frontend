# 🎯 YouTube Comment Sentiment Analyzer (Chrome Extension)

This project is a **Chrome extension** that fetches YouTube video comments, performs **sentiment analysis using ML models**, and visualizes results with graphs and statistics. The backend is a **Flask API deployed on Render**, integrated with **MLflow & DVC** for model management.

---

## **👁‍🗨 1. Clone the Frontend Repository**
To get started, clone the frontend repository:

```bash
git clone https://github.com/aryan0147/Capstone-2-frontend.git
cd Capstone-2-frontend
```

---

## **🔑 2. Get a YouTube API Key**
This extension uses the **YouTube Data API v3** to fetch video comments. Follow these steps to get an API key:

### **Step 1: Go to Google Cloud Console**
- Open [Google Cloud Console](https://console.cloud.google.com/).
- Sign in with your Google account.

### **Step 2: Create a New Project**
- Click on the project dropdown (top-left) → "New Project".
- Give your project a name (e.g., **YouTube-Sentiment-Analysis**).
- Click **Create** and wait for the project to be created.

### **Step 3: Enable the YouTube Data API**
- In the **API & Services** dashboard, click "Enable APIs & Services".
- Search for **YouTube Data API v3** and **enable it**.

### **Step 4: Generate API Key**
- In the left sidebar, go to **Credentials**.
- Click **Create Credentials** → Select **API Key**.
- Copy the generated API Key (you will need this in `popup.js`).

---

## **📝 3. Add the API Key to `popup.js`**
Once you have the API key, open `popup.js` in the frontend repo and **replace** this line:

```js
const API_KEY = 'YOUR_YOUTUBE_API_KEY_HERE';
```

With **your actual API key**:

```js
const API_KEY = 'AIzaSyXXXXXX-Your-API-Key-Here';
```

---

## **🚀 4. Load the Extension in Chrome**
1. Open **Google Chrome**.
2. Go to `chrome://extensions/`.
3. Enable **Developer mode** (toggle in the top-right).
4. Click **"Load unpacked"**.
5. Select the **`Capstone-2-frontend`** folder.
6. The extension should now be loaded!

---

## **🔠 5. Test the Extension**
1. Open **YouTube** and go to any video.
2. Click the **YouTube Sentiment Analyzer** extension icon.
3. It will fetch comments, analyze sentiments, and display the results!

---

## **💡 Need Help?**
If you face any issues, feel free to raise an issue in the GitHub repo or contact me! 🚀

