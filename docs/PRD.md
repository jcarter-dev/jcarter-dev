# PRD: AI UI Theme Generator for Java Swing

## 1. Project Overview
This project is a simple web-based tool that helps users generate UI themes for Java Swing applications. The user types a short description of the look they want (for example: “teal glass theme,” “dark mode with cyan accents,” or “retro terminal green”), and the page outputs a set of color values and UI constants they can drop into their Java code.  

**Target User:**  
Students or developers working on Java Swing projects who want faster, more consistent theme creation.

**Problem It Solves:**  
Styling Swing apps is repetitive and kind of annoying. You end up tweaking the same colors and constants in multiple places. This tool speeds that up and makes it easier to explore different looks without rewriting everything by hand.

---

## 2. Core Features (MVP)

### Feature 1: Theme Description Input
**What it does:**  
Lets the user type a short description of the theme they want.

**Why it matters:**  
This is how the user tells the tool what kind of style they’re going for.

**Success Criteria:**  
The page accepts text input and uses it to update the generated theme.

---

### Feature 2: Generated Theme Output
**What it does:**  
Based on the description, the page shows:
- Primary color  
- Secondary color  
- Accent color  
- Background color  
- A small preview box using those colors  

**Why it matters:**  
This gives the user something concrete they can copy into their Swing project.

**Success Criteria:**  
The values are displayed clearly and the preview updates when the user generates a new theme.

---

### Feature 3 (Nice-to-have for MVP): Copy Theme Snippet
**What it does:**  
Provides a “Copy theme snippet” button that copies a small block of text with the color constants.

**Why it matters:**  
Makes it easier to move the theme into Java code with as little friction as possible.

**Success Criteria:**  
Clicking the button copies the snippet to the clipboard.

---

## 3. User Experience

**First screen:**  
- A short title and description  
- One text box: “Describe your theme…”  
- A “Generate Theme” button  
- An empty preview area the first time

**Typical flow:**
1. User types a short description of the theme.
2. User clicks “Generate Theme.”
3. The preview and color values appear.
4. User can tweak the text and regenerate as many times as they want.
5. (Optional) User clicks “Copy theme snippet” to grab the values.

---

## 4. Technical Constraints

- Single-page application: just **one** HTML file with embedded CSS and JavaScript.
- Must run directly in a browser (no server, no build step required).
- No external libraries required for the MVP.
- Logic for generating themes can be simple (for v1 it doesn’t have to be “real AI” — can be rule-based or basic mapping).
- Should be easy to modify later if I want to plug in an actual AI backend.

---

## 5. Out of Scope for v1

These are intentionally **not** part of the MVP:

- Real-time integration with a Java project or IDE.
- User accounts, saving/loading themes to a database.
- Advanced color accessibility checks or contrast validation.
- Complex AI model integration (like calling an API from the browser).
- Multi-page navigation or settings panels.

These are future ideas for a bigger version once the basic MVP is stable.

---

## Summary

For this MVP, I’m focusing on a small, clear tool: take a short text description and turn it into a simple, consistent theme preview for Java Swing. It should be easy to open in a browser, easy to understand, and realistic to build in one short sprint.
