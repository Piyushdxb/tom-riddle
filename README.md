
# 🪄 Tom Riddle's Diary — Interactive Web & iPad Edition

An interactive, web-based recreation of **Tom Riddle’s Diary** from *Harry Potter and the Chamber of Secrets*. Write on the page with your stylus or finger, pause, and watch the parchment "drink" your ink. Moments later, the diary thinks, and Tom Riddle answers back in an animated, flowing cursive hand.

This project is a zero-dependency, single-file HTML5 web application optimized for the **iPad & Apple Pencil**, inspired by [MaximeRivest's open-source Rust project](https://github.com/MaximeRivest/riddle) for the reMarkable Paper Pro.

---

## ✨ Key Features

* **Apple Pencil & Touch Optimized:** Built with HTML5 Canvas Retina scaling and pointer event locking (`touch-action: none`) so you can rest your hand and draw smoothly without accidentally scrolling the page.
* **The "Drinking Ink" Effect:** When you pause writing for 2.5 seconds, your handwriting smoothly fades into the e-ink parchment background.
* **AI Vision Oracle (OpenAI):** Connects directly to OpenAI's `gpt-4o-mini` Vision API. The AI actually *reads* your handwritten message from an inline image capture and responds in character as the sentient memory of Tom Riddle.
* **Offline / Fallback Mode:** No API key or internet connection? No problem. The app automatically falls back to a curated library of spooky, built-in Tom Riddle memories so you can use it anytime, anywhere.
* **Animated Cursive Script:** Responses write themselves onto the screen letter-by-letter using the flowing *Dancing Script* font before fading away clean for your next entry.

---

## 🚀 How to Use & Play

1. **Write:** Use your stylus, finger, or mouse to write a question or thought on the blank page.
2. **Rest Your Pen:** Stop writing for **2.5 seconds**. 
3. **The Drink:** The ink will blur and dissolve into the paper.
4. **The Reply:** Watch as Tom Riddle writes his reply back to you in real-time. Once you finish reading (after ~6 seconds), the page wipes clean automatically.

---

## 📱 iPad Setup (Full-Screen "Native App" Experience)

To get the best experience without Safari URL bars or browser buttons cluttering the screen:

1. Visit the live GitHub Pages URL for this repository in **Safari on your iPad**:
   `(https://piyushdxb.github.io/tom-riddle/)`
2. Tap the **Share button** (the square with the upward arrow) in the Safari toolbar.
3. Scroll down and select **Add to Home Screen**.
4. Name it **The Diary** and tap **Add**.
5. Launch the app directly from your iPad home screen! It will open in full-screen mode, feeling exactly like a native iPad app.

---

## 🔮 Configuring the AI Oracle (OpenAI Vision)

By default, the diary uses pre-programmed fallback quotes. To let Tom Riddle actually read your handwriting and generate custom responses:

1. Open the app and tap the subtle **🪄 (Wand Icon)** in the top right corner of the screen.
2. Paste your OpenAI API Key (starts with `sk-...`).
3. Tap **Save & Close**.

> **🔒 Privacy Note:** Your API key is stored locally and securely in your device's browser memory (`localStorage`). It is never sent to any third-party servers—it only communicates directly between your device and OpenAI's API endpoints.

---

## 🛠️ Offline Usage

If you want to use the app 100% offline without an internet connection:

1. Download the `index.html` file to your iPad's local **Files** app.
2. Download a free offline code viewer or lightweight editor from the App Store (such as **Koder** or **Documents by Readdle**).
3. Open `index.html` inside the app using its built-in browser preview.
*(Note: When offline, the app automatically switches to the built-in quote library instead of the OpenAI cloud API).*

---

## 📜 Acknowledgments & Disclaimer

* Original hardware concept and inspiration by [MaximeRivest's Riddle for reMarkable Paper Pro](https://github.com/MaximeRivest/riddle).
* Cursive font provided by [Google Fonts (Dancing Script)](https://fonts.google.com/specimen/Dancing+Script).
* *Harry Potter*, Tom Riddle, and related properties are trademarks of J.K. Rowling and Warner Bros. Entertainment Inc. This is an unofficial, fan-made open-source project created for educational and entertainment purposes.
