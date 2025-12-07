# AI UI Theme Generator (MVP)

This project is my MVP for CSC-113. The goal was to take a simple idea — “describe a vibe and get a matching Java Swing theme” — and turn it into a working prototype using a rapid-prototyping workflow. Everything runs in a single HTML file, and it updates the preview instantly based on the user’s description.

---

## What the App Does

- Lets the user type a short theme description  
- Matches the description to a preset (keywords like teal, retro, terminal, neon, etc.)  
- Generates a color palette: primary, secondary, accent, background  
- Updates a small Swing-style preview panel so you can *see* the theme  
- Produces ready-to-paste Java color constants  
- Includes a “copy snippet” button for convenience  

No backend, no installs — you just open `index.html` in a browser.  

---

## How to Use

1. Open `index.html` in any browser  
2. Write a short description of the theme you want  
3. Click **Generate Theme**  
4. The preview and color values update instantly  
5. Copy the Java snippet and drop it into your Swing UI code  

---

## Files Included

- **PRD.md** – The product requirements document  
- **index.html** – Final MVP app  
- **PROTOTYPE_TESTING.md** – Notes comparing ChatGPT vs. Gemini versions  
- **ITERATION_LOG.md** – Log of fixes, adjustments, and refinement  
- **prototypes/** – Folder holding the raw prototype HTML files  
- **README.md** – This documentation  

---

## Development Summary

I generated two different prototypes (ChatGPT and Gemini) based on the same PRD.  
After testing them side-by-side, I took the stronger version and iterated until:

- Colors updated consistently  
- The preview panel matched the generated values  
- Java snippets were formatted clearly  
- The layout scaled better  

My logs show each step taken to fix issues and improve the final result.

---

## What I Learned

- How the same PRD can lead to completely different prototype outputs  
- Why small, focused iterations are better than trying to rewrite everything at once  
- How to debug UI behavior in a simple HTML/CSS/JS environment  
- How to use GitHub issues, branches, and PRs in an actual workflow  
- How to build something quickly without overthinking every detail  

---

## Future Improvements

- Add manual color pickers  
- Add a downloadable theme preset file  
- Let users save multiple generated themes  
- Allow LLM-based palette generation instead of keyword matching  
- Add animations or smoother transitions in the preview panel  

---

## Live Demo

(Will be added after enabling GitHub Pages.)
