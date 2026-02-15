## Anuroop Brahmanand HK – Portfolio

This is a single-page portfolio website built with **HTML**, **Tailwind CSS (CDN)**, and a few lines of vanilla **JavaScript**.  
It presents your resume as a series of **horizontal slides** with smooth left-to-right transitions, glowing purple cards, and a **cursor spotlight** effect that follows the pointer.

---

### Features

- **Purple & white visual identity**
  - Gradient background from deep purple to black.
  - Cards in a soft light-purple shade (matching the requested card color).
- **Enlarged profile image**
  - Prominent hero card with your photo, glow, and hover zoom.
  - Replace the image at `./assets/profile.jpg` with your real profile picture.
- **Horizontal slide layout**
  - Sections: `Home`, `About`, `Education`, `Projects`, `Skills`, `Community`, and `Contact`.
  - Left/right navigation using:
    - Top navigation buttons,
    - Bottom arrow controls,
    - Horizontal scrolling (mouse/trackpad/swipe).
- **Cursor spotlight**
  - A soft radial highlight that follows the pointer across the page.
- **Responsive design**
  - Mobile-friendly layout with stacked content and a compact mobile menu.
- **Contact & enquiry**
  - Contact form that opens a **Gmail message** to `ab.anuroop@gmail.com` via `mailto`.
  - Direct social links to your LinkedIn and GitHub profiles.

---

### Running the Project Locally

Prerequisites:

- Node.js (LTS) and npm installed.

Steps:

1. Navigate to the project folder:

   ```bash
   cd d:\MY_PRJ
   ```

2. Install dependencies (already done if you see `node_modules`):

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

4. Your default browser should open the site at a local URL (for example: `http://127.0.0.1:8080`). If not, open the URL printed in the terminal manually.

---

### Preparing Assets

- Create an `assets` folder in the project root if it does not exist.
- Save your profile photo as:

  ```text
  d:\MY_PRJ\assets\profile.jpg
  ```

- Adjust the path in `index.html` if you prefer a different filename or format.

---

### Deploying to GitHub

1. Initialize git in the project (if not already):

   ```bash
   cd d:\MY_PRJ
   git init
   git add .
   git commit -m "Initial portfolio site"
   ```

2. On GitHub, create a new empty repository (for example: `portfolio`).

3. Connect the local repo to GitHub:

   ```bash
   git remote add origin https://github.com/anuroop0099/portfolio.git
   git branch -M main
   git push -u origin main
   ```

After that, every time you run:

```bash
git add .
git commit -m "Update portfolio"
git push
```

GitHub will stay in sync with your latest changes.

---

### Deploying to Vercel (Automatic)

1. Go to [`https://vercel.com`](https://vercel.com) and sign in with GitHub.
2. Click **"New Project"** and import your `portfolio` repository.
3. Build settings:
   - Framework: **Other** / **Static** (no special build command needed).
   - Build command: leave empty.
   - Output directory: `/` (project root).
4. Click **Deploy**.

Once deployed:

- Vercel will give you a live URL (e.g. `https://anuroop-portfolio.vercel.app`).
- Every `git push` to `main` will trigger an **automatic deployment** — no extra manual steps.

---

### Basic Manual Testing Checklist

- **Layout & responsiveness**
  - Check the site on mobile, tablet, and desktop widths.
  - Ensure horizontal slides are scrollable and content is readable.
- **Navigation**
  - Top navigation buttons jump to the correct slide.
  - Left/right arrow buttons move between sections smoothly.
- **Interactions**
  - Cursor spotlight follows the mouse.
  - Cards lift and glow on hover.
  - Profile image zooms slightly on hover.
- **Contact**
  - Submitting the contact form opens a new email in your default mail app addressed to `ab.anuroop@gmail.com` with the filled-in details.

This project is ready to demonstrate your skills, attention to detail, and sense of design to your company head and any future recruiters.

