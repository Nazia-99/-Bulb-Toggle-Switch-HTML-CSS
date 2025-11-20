# 💡 Bulb Toggle Switch | HTML & CSS
# 💡 Bulb Toggle Switch | HTML & CSS

A unique and realistic **bulb-style toggle switch** built using only **HTML & CSS**.  
It mimics the look of a real light switch — complete with a lever-style handle and glowing bulb effect when turned on!

---

## 🧠 Features

✔ Pure **HTML & CSS** (No JavaScript)  
✔ Realistic **lever/bulb effect**  
✔ Smooth **animation & transition**  
✔ Fully **responsive**  
✔ Easy to **add in any project**

---

## 📦 Source Code

### 🔹 `index.html`
```html
<label>
  <input type="checkbox" class="bulb-toggle" />
</label>
.bulb-toggle {
  width: 3em;
  height: 1.5em;
  border-radius: 0.75em;
  background-color: rgba(0,0,0,0.7);
  box-shadow: inset 0.125em 0.125em 0 0.125em rgba(0,0,0,0.3);
  padding: 0.15em;
  display: inline-flex;
  align-items: center;
  appearance: none;
  cursor: pointer;
  transition: background-color 0.1s 0.3s ease-out, box-shadow 0.1s 0.3s ease-out;
}

.bulb-toggle::before {
  content: "";
  width: 1.2em;
  height: 1.2em;
  border-radius: 50%;
  background-color: #d7d7d7;
  transition: background-color 0.1s 0.3s ease-out, transform 0.3s ease-out;
}

.bulb-toggle::after {
  content: "";
  width: 1.2em;
  height: 1.2em;
  transform: translateX(-22.5%);
  transform-origin: 25% 60%;
  background:
    linear-gradient(transparent 50%, rgba(0,0,0,0.15) 0) 0 50% / 50% 100%,
    repeating-linear-gradient(90deg, #bbb 0, #bbb 20%, #999 20%, #999 40%) 0 50% / 50% 100%,
    radial-gradient(circle at 50% 50%, #888 25%, transparent 26%);
  background-repeat: no-repeat;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
  border: 0.25em solid transparent;
  border-left: 0.4em solid #d8d8d8;
  transition: border-left-color 0.1s 0.3s ease-out, transform 0.3s ease-out;
}

.bulb-toggle:checked {
  background-color: rgba(0,0,0,0.45);
  box-shadow: inset 0.125em 0.125em 0 0.125em rgba(0,0,0,0.1);
}

.bulb-toggle:checked::before {
  background-color: #f8dd44;
  transform: translateX(125%);
}

.bulb-toggle:checked::after {
  border-left-color: #f8dd44;
  transform: translateX(-2.5%) rotateY(180deg);
}


**** 🔧 How to Use

Copy the HTML and CSS files.

Link style.css in your HTML using:

<link rel="stylesheet" href="style.css">


Done! Your toggle switch is ready to use.

⭐ Support

If this helped you, give it a star ⭐ on GitHub!
More awesome UI coming soon — Follow me! 😄

🧷 License

MIT License – Free to use for personal & commercial projects.

📌 Author

👩‍💻 Nazia
YouTube: Code With Nazia
