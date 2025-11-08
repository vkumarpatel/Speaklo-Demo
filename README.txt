
Speaklo Demo — ZIP package
=========================

Files:
- index.html          -> Demo page (Lottie avatar + TTS + mic start/stop)
- README.txt          -> This file (instructions)

How to use:
1) Quick local test (no server required):
   - Open the file 'index.html' in Chrome (desktop) or serve via a local static server:
     * Recommended: from project folder run:
         npx serve .
       then open http://localhost:5000 in Chrome.
   - Click 'Start Mic' — grant microphone permission when prompted.
   - Speak; mouth animation should respond. Click 'Stop Mic' to stop.
   - Use 'Play Sample' or 'Play Welcome' to test TTS. Use Voice dropdown to pick available voices.

2) Deploy (recommended):
   - Push the files to a GitHub repo and deploy via Vercel (free). Vercel provides HTTPS automatically so mic works on mobile.
   - Or host the folder on any static hosting (Netlify, GitHub Pages).

Notes / Troubleshooting:
- Microphone requires HTTPS or localhost. If you open file:// in browser, mic will not work.
- If you previously blocked mic permission, go to browser site settings and allow microphone for the site.
- TTS voices depend on the browser and OS. Chrome/Edge usually have better voices. If no voices appear, wait a few seconds after page load, or refresh.
- Lottie is loaded from a public URL. If you want to use a local Lottie JSON, replace LOTTIE_JSON in the index.html with the local path to your JSON file.

Need help?
- If you want, paste your GitHub repo URL and I can deploy to Vercel for you and test it live.
- If anything fails, copy any console errors from DevTools and paste them here. I'll debug further.
