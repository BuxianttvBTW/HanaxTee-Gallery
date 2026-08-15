================================================================
  💕 Hello Kitty Love Website — for your girl 💕
================================================================

PROJECT STRUCTURE
-----------------
   index.html       — the whole site (open this in a browser)
   gifs/            — 11 cute Hello Kitty & Dear Daniel GIFs (local, works offline)
   photos/          — drop YOUR 30 photos here, named 1.jpg ... 30.jpg
   README.txt       — this file


HOW TO DEPLOY ON GITHUB PAGES
-----------------------------
1. Create a new GitHub repo (e.g. `hello-kitty-love` or `for-my-love`).

2. Push everything in this folder to the repo:
       git init
       git add .
       git commit -m "💕"
       git branch -M main
       git remote add origin https://github.com/YOUR-USER/REPO.git
       git push -u origin main

3. On GitHub: repo → Settings → Pages → Source: `main` branch, root.
   Wait ~1 minute. Your site will be live at:
       https://YOUR-USER.github.io/REPO/

4. Send her the link. She opens it, types `2407`, done. 💕


HOW TO ADD YOUR 30 PHOTOS
-------------------------
Drop your photo files into the `photos/` folder using the exact names:

       photos/1.jpg   photos/2.jpg   photos/3.jpg   ...   photos/30.jpg

Supported: .jpg, .jpeg, .png, .webp  (case doesn't matter)

You don't have to use all 30. Empty slots show a cute Hello Kitty
placeholder GIF automatically.

       git add photos/
       git commit -m "📸 added our photos"
       git push

That's it. The site reloads, and your photos are there. 💕

TIP: Use roughly square (1:1) photos — the album frame is a square.


RUNNING LOCALLY (OPTIONAL)
--------------------------
Just double-click `index.html` — it works in any browser, no build,
no install, no server needed. (Tip: if you want the photos/ folder
to work, run it through a tiny local server, since some browsers
block local file:// photos. Easiest: `python3 -m http.server` in
this folder, then visit http://localhost:8000.)


CUSTOMIZE
---------
• Change the "started on" date (currently 13 November 2025):
  Open index.html → search for `new Date("2025-11-13` → edit the date.

• Change the password (currently 2407):
  Open index.html → search for `const PASSWORD = "2407"` → replace.

• Edit the love letter:
  Open index.html → search for "A Little Note For You" → rewrite the
  paragraphs inside the `<div class="letter">` block.

• Edit the "Reasons I Love You" cards:
  Open index.html → search for `reason-card` → rewrite each card.

• Add background music:
  At the very bottom of <body> (just before `</body>`) paste:
      <audio autoplay loop>
        <source src="your-song.mp3" type="audio/mpeg">
      </audio>
  Then drop your-song.mp3 next to index.html, commit, push.


WHAT'S IN THE SITE
------------------
• 🔐 Password lock screen (cute keypad + Dear Daniel GIF)
• 💖 Hero with Hello Kitty & Dear Daniel side-by-side
• 🗓️ Live "days together" counter (updates every minute)
• 💌 Handwritten-style love letter on pink notebook paper
• 💕 "Reasons I Love You" cards
• 📸 30-photo swipeable album
       — swipe on mobile, drag on desktop, or use the arrow buttons
       — tap a photo to expand it full-screen
       — keyboard arrow keys also work
       — "Add / Change Photo" lets you upload from your device too
       — "Auto-play" cycles through the photos like a slideshow
       — "Reset All Photos" only clears browser uploads (not photos/)
• ✨ "You're My Forever" finale
• 🎵 Floating music player — "Until I Found You" by Stephen Sanchez
       (YouTube-powered so it works on GitHub Pages for free.
        To change the song, edit `YT_VIDEO_ID` in the JS — the value
        is the part after `?v=` in any YouTube link.)
• 🌸 Floating hearts background + tap-for-heart-burst
• 💗 Custom pink heart cursor on desktop

================================================================
Made with 💕 · enjoy
================================================================
