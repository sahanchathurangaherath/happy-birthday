# 🎂 Cutiee's Interactive Birthday Website ♡

A responsive, multi-step romantic birthday website crafted with soft pastel cream/blush tones, smooth transitions, interactive animations, sound effects, and romantic lo-fi background music.

---

## ✨ Features & Interactive Steps

1. **Step 1: The Sealed Envelope (Intro)**
   - "MADE WITH SO MUCH LOVE" header badge with gentle float animation.
   - "Hello Cutiee" title with cursive subtitle.
   - Cute dancing party bear mascot with birthday hat.
   - Interactive 3D envelope with a pulsing wax seal button (`#b91c1c`).
   - Clicking the seal plays an unseal chime, unfolds the envelope flap, bursts sparkles, gently starts the music, and smoothly transitions to Step 2.
   - Canvas background with drifting cherry blossom petals and floating sparkles.

2. **Step 2: The Welcome & Mini Music Player**
   - Cute chibi couple character avatar with a playful "HEHEEE ♡" badge.
   - "Happy Birthday My Madam Jii ♡" title & heartfelt message box.
   - Mini Music Player:
     - Spinning vinyl album art badge with animated equalizer wave bars.
     - Play/Pause toggle button.
     - Interactive scrubber time bar and elapsed/total duration counter.
     - Caption: *"I picked this one, because it always reminds me of you."*
   - CTA button: "SEE OUR ALBUM →".

3. **Step 3: Interactive Memory Polaroid Carousel**
   - Washi-tape pinned polaroid card.
   - Memory indicator (`MEMORY 01 / 03`).
   - Next/Previous arrow controls + **touch swipe support** on mobile and tablets.
   - 3 pre-loaded cute slides with illustrations & captions (Inside jokes, birthday wishes, cuddly moments).
   - CTA button: "PICK A WISH →".

4. **Step 4: "A Tiny Bouquet of Birthday Wishes"**
   - 3 flower cards (Rose, Daisy, Cherry Blossom) in front of an illustrated ceramic pot.
   - "PICK ME" prompt with bounce animations.
   - Clicking flips each card with a 3D animation, plays a chime, and reveals a hidden sweet wish.
   - Dynamic counter tracks opened flowers.
   - Unlocking all 3 flowers reveals the "READ MY LETTER →" button.

5. **Step 5: The Final Birthday Letter**
   - Elegant header pill and cute chibi avatar badge.
   - Heartfelt, warm love letter with beautiful typography (`Playfair Display`, `Caveat`, `Quicksand`).
   - "Your Biggest Fan ♡" signature with an embossed wax stamp badge.
   - **"CLICK FOR BIRTHDAY RAIN & CELEBRATION! 🎉"** button: Triggers full-screen heart confetti cannons and sparkle sounds!
   - Restart journey button to experience it all over again.

---

## 🚀 How to Run the Website

### Option 1: Double-Click
Simply double-click `index.html` in your file explorer to open it in Chrome, Safari, Edge, or Firefox.

### Option 2: Live Local Server
Run this command in the project folder:
```powershell
python -m http.server 8000
```
Then visit: `http://localhost:8000`

---

## 📸 How to Add Her Photos Using Code

Open [`index.html`](file:///c:/Users/Sahan/Documents/antigravity/eager-lavoisier/index.html) and go to line **1305** (inside the `<script>` tag).

You will see the `slidesData` array:

```javascript
const slidesData = [
  {
    tag: 'MEMORY 01 / 03',
    photo: 'images/photo1.jpg', // <-- Put your photo path or web link here
    caption: '"The day we couldn\'t stop laughing at the silly jokes"',
    sub: 'Every little smile of yours brightens my whole world ♡'
  },
  {
    tag: 'MEMORY 02 / 03',
    photo: 'images/photo2.jpg', // <-- Put your photo path or web link here
    caption: '"Making wishes together & celebrating YOU"',
    sub: 'I hope every dream you hold close comes true this year! 🎂'
  },
  {
    tag: 'MEMORY 03 / 03',
    photo: 'images/photo3.jpg', // <-- Put your photo path or web link here
    caption: '"You when you get your favourite snacks 🍕"',
    sub: 'My adorable, hungry little cutiee who always steals my fries ♡'
  }
];
```

### 2 Ways to set the photo path:
1. **Using local images**: Copy your photos into the `images/` folder (e.g. `images/her1.jpg`, `images/her2.jpg`) and write:
   ```javascript
   photo: 'images/her1.jpg',
   ```
2. **Using image links from the web / Google Drive / Imgur / Cloudinary**:
   ```javascript
   photo: 'https://i.imgur.com/example.jpg',
   ```

*(Note: If a photo is not found or fails to load, the website automatically falls back to the cute cartoon drawings so nothing looks broken!)*
