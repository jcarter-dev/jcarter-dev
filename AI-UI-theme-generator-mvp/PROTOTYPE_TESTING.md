# Prototype Testing & Comparison

I generated two different prototypes based on the same PRD: one using ChatGPT and one using Gemini.  
Originally, I tried to test them inside GitHub Codespaces, but the preview kept redirecting me to `index.html`, so I downloaded each file and tested them locally in my browser.

---

## Version 1: ChatGPT Prototype

### ✅ What Works
- The main layout loads correctly with the input box and the preview panel side-by-side.
- Theme colors update visually when the generator is used.
- The Java Swing snippet updates after generating a theme.
- Buttons respond and don’t break the page.

### ❌ What’s Broken / Not Ideal
- Color generation is sometimes inconsistent (same prompt gave slightly different tones).
- Some UI spacing feels tight or misaligned.
- The preview “dashboard mockup” doesn’t always match the selected accent color.
- Code formatting in the snippet box is readable, but not super clean.

### 💭 Observations
- ChatGPT’s version looks the most polished visually.
- It seems more “designed,” but maybe a little over-styled for a first MVP.
- Logic is straightforward and commented clearly enough to follow.

---

## Version 2: Gemini Prototype

### ✅ What Works
- Page loads cleanly and without console errors.
- The theme generator updates the color values (primary / secondary / accent).
- The Java code snippet updates reliably.
- Simpler structure makes it easier to read the JS logic.

### ❌ What’s Broken / Not Ideal
- The preview UI is *very* minimal — almost too plain.
- Some input elements don’t respond visually when hovered or clicked.
- Color preview blocks sometimes don’t match the generated values perfectly.
- No fallback styling if the model can't parse the prompt.

### 💭 Observations
- Gemini produced a simpler, more “barebones” prototype.
- Easier to debug because the JS is short and clear.
- Not as visually appealing, but feels stable.

---

## ⭐ Decision

I’m choosing **ChatGPT’s prototype as my base MVP**.

### Reasoning:
- Better overall layout and user flow.
- The preview panel feels closer to the final product vision.
- More intuitive UX for a first-time user.
- Less work needed to get it looking “portfolio ready.”

Gemini’s version is still useful as a reference, especially for simplifying the JS logic if I need to debug later.

---

## Summary

Both prototypes technically worked, but each had strengths and issues.  
ChatGPT’s felt closest to what I envisioned in the PRD, so I’m moving forward with that as the foundation.
