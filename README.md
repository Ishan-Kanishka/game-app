cat << 'EOF' >> README.md

# Game App — Angular Setup Notes

## 1. Installed Node.js
- Downloaded from: [https://nodejs.org](https://nodejs.org)
- Installed **LTS (Long Term Support)** version.
- Verified installation:
```bash
node -v    # Check Node.js version
npm -v     # Check npm version
```

---

## 2. Installed Angular CLI Globally
```bash
npm install -g @angular/cli
```
- Verified installation:
```bash
ng version
```

---

## 3. Created New Angular Project
```bash
ng new game-app
```
**CLI Prompts & Answers:**
1. **Do you want to create a zoneless app without zone.js?** → **No**  
   *Reason:* Keeping `zone.js` is easier for beginners; it auto-detects UI changes.  
2. **Would you like to add Angular routing?** → **Yes**  
   *Reason:* Allows navigation between pages/components (e.g., Home, Game).  
3. **Which stylesheet format would you like to use?** → **CSS**  
   *Reason:* Simple for starting; can switch to SCSS later if needed.  
4. **Do you want to enable SSR (Server-Side Rendering)?** → **No**  
   *Reason:* Not needed for a small SPA game; avoids extra complexity.

---

## 4. Navigated into Project Folder
```bash
cd game-app
```

---

## 5. Started Development Server
```bash
ng serve
```
- App available at: **http://localhost:4200**

---

## 6. Project Structure Overview
Key files inside `src/app`:
- **app.component.ts** → Main component logic (TypeScript)
- **app.component.html** → Main HTML template
- **app.component.css** → Styles for main component
- **app.module.ts** → Registers components & modules

---

## Next Step
Create a **Game Component** to add a Flappy Bird-like game using `<canvas>`.

EOF
