# 🤖 Gemini AI Clone

A browser-based conversational AI clone that replicates the look and feel of Google's Gemini interface — built with HTML, CSS, and JavaScript, and powered by the Gemini API.

---

## 📌 Overview

This project is a functional clone of the Gemini AI chat interface. It features a greeting header, 4 pre-built prompt suggestion cards, a live chat conversation area, a prompt input field with a send button, a light/dark theme toggle, and a delete chat button. All chat logic and API communication are handled in `Script.js`. The `Assets/` folder holds local images used in the interface.

---

## ✨ Features

- **Greeting Header** — On load, the app displays a welcome message `"Hello, there"` with the subtitle `"How can I help you today?"`, matching Gemini's actual UI pattern.
- **4 Prompt Suggestion Cards** — Pre-written prompt cards are shown before the user starts chatting, each with a Material Symbols icon:
  1. 🖊️ *"Help me plan a game night with my 5 best friends for under $100."* — `draw` icon
  2. 💡 *"What are the best tips to improve my public speaking skills?"* — `lightbulb` icon
  3. 🔍 *"Can you help me find the latest news on web development?"* — `explore` icon
  4. 💻 *"Write JavaScript code to sum all elements in an array."* — `code` icon
- **Live Chat List (`.chat-list`)** — User messages and AI responses are dynamically rendered into the chat area by JavaScript. The suggestion header hides once a conversation starts.
- **Prompt Input Field** — A text input (`typing-input`) with placeholder `"Enter a prompt here"` accepts user messages. The field is marked `required` so empty submissions are blocked.
- **Send Button** — A Material Symbol `send` icon button submits the typed prompt to the Gemini API via JavaScript.
- **Light / Dark Theme Toggle (`#toggle-Theme-button`)** — A `light_mode` Material Symbol icon toggles between light and dark themes. The selected theme preference is applied across the full interface.
- **Delete Chat Button (`#delete-chat-button`)** — A `delete` icon button clears the entire conversation history from the chat list and resets the UI back to the initial suggestion view.
- **Gemini API Integration** — `Script.js` sends the user's prompt to the Gemini API and streams or renders the response back into the `.chat-list` in real time.
- **Disclaimer Text** — A footer note reads: *"Gemini may display inaccurate info, including about people, so double-check its responses."* — keeping the experience authentic to the original product.
- **Google Material Symbols Rounded Icons** — All icons (send, light_mode, delete, draw, lightbulb, explore, code) are loaded via Google Fonts CDN with no extra icon library needed.
- **Local Assets Folder** — The `Assets/` directory stores any local images or visual resources used by the interface.
- **Responsive Design** — CSS media queries ensure the layout works cleanly across desktop, tablet, and mobile screen sizes.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure — header, suggestion cards, chat list, typing area, action buttons |
| CSS3 | Gemini-style UI, theme switching, responsive layout |
| JavaScript (ES6+) | Gemini API calls, response rendering, theme toggle, chat deletion, DOM management |
| Gemini API | AI responses to user prompts |
| Google Material Symbols Rounded | All UI icons loaded via Google Fonts CDN |

---

## 📁 Project Structure

```
Gemini-Ai/
├── Index.html      # Main HTML — header, 4 suggestion cards, chat list, input form, action buttons
├── Style.css       # Full UI styling — Gemini-inspired layout, dark/light theme, responsive design
├── Script.js       # Core logic — API integration, chat rendering, theme toggle, delete chat
├── Assets/         # Local images and visual assets used in the interface
└── README.md       # Project documentation
```

---

## 🚀 Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/tripathipawan/Gemini-Ai.git
```

**2. Navigate into the project folder**
```bash
cd Gemini-Ai
```

**3. Add your Gemini API key**

Open `Script.js` and add your API key in the designated variable. You can get a free key from [Google AI Studio](https://aistudio.google.com/).

**4. Open in browser**
```
Open Index.html in any modern browser
— or use VS Code Live Server
```

> **Note:** An active internet connection is required for the Gemini API and Google Fonts CDN icons to load.

---

## 🧭 How to Use

1. Open the app — the greeting header and 4 suggestion cards appear.
2. Click a suggestion card to auto-fill the prompt, or type your own in the input field.
3. Click the **send** button to submit your message.
4. The AI response appears in the `.chat-list` area below the input.
5. Click the **🌙 / ☀️ theme icon** to toggle between dark and light mode.
6. Click the **🗑️ delete icon** to clear the entire chat and return to the suggestion view.

---

## 🌱 What I Learned

- Integrating Google's Gemini API to send prompts and handle streamed or batch AI responses
- Building a multi-state UI that transitions from a suggestion view to a live chat interface
- Implementing a persistent light/dark theme toggle using JavaScript and CSS class switching
- Rendering dynamic conversation threads into the DOM without a framework
- Using Google Material Symbols Rounded via CDN as a lightweight icon system

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Commit your changes (`git commit -m 'Add: your feature description'`)
4. Push to the branch (`git push origin feature/your-feature-name`)
5. Open a Pull Request

---

## 👨‍💻 Author

**Pawan Tripathi**
- GitHub: [@tripathipawan](https://github.com/tripathipawan)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
