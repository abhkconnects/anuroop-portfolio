## Portfolio Website Roadmap

This roadmap describes how to build, test, and deploy your portfolio site based on your resume, using Tailwind CSS, a purple/white theme, and automated deployment to GitHub and Vercel.

---

### Phase 1: Planning (Current Phase — No Implementation Yet)

- **Define content from resume**
  - List sections: About, Education, Skills, Projects, Experience, Achievements/Certifications, Contact.
  - For each project/experience, decide: title, role, tech stack, 2–3 bullet highlights, links (GitHub, live demo).
- **Decide visual style**
  - Primary palette: purple and white (e.g. purple \#7C3AED, light background \#F9FAFB).
  - Card background shade: light purple (e.g. \#EDE9FE).
  - Enlarged profile photo on hero section.
- **Interaction & navigation**
  - Single-page layout split into “slides” (sections) that move from left to right.
  - Smooth transitions when navigating between sections.

---

### Phase 2: Project Setup

- **Initialize project**
  - Create a new Git repository in the project folder.
  - Choose a framework:
    - Option A (simple): plain HTML + Tailwind via CDN.
    - Option B (recommended): Next.js + Tailwind CSS for better routing and deployment with Vercel.
- **Install Tailwind CSS**
  - If using Next.js, install Tailwind via official setup guide.
  - Configure Tailwind theme with custom purple color and card shade.
- **Base structure**
  - Create main layout with:
    - `Header` (name, logo, navigation).
    - `Main` area containing horizontal “slides” for each section.
    - `Footer` (links, copyright).

---

### Phase 3: Layout & Flow (Implement Flow From Resume)

- **Hero / Introduction slide**
  - Large profile picture (enlarged compared to other content).
  - Name, title, short 2–3 sentence summary.
  - Call-to-action buttons: “View Projects”, “Download Resume”.
- **Sections as slides (left-to-right)**
  - Slide 1: About + Education.
  - Slide 2: Skills (grouped by category: languages, frameworks, tools).
  - Slide 3: Projects (each as a purple-shaded card).
  - Slide 4: Experience / Internships (timeline style).
  - Slide 5: Achievements / Certifications.
  - Slide 6: Contact (form or email/social links).
- **Flowchart alignment**
  - Ensure visual order of sections matches the flowchart you designed (Career journey: Start → About → Education → Skills → Projects → Experience → Achievements → Contact).

---

### Phase 4: Styling & Responsiveness

- **Tailwind styling**
  - Apply purple/white theme to backgrounds, text, buttons, and cards.
  - Use the specified card shade for all project/experience cards.
  - Ensure focus states and hover effects are clear and accessible.
- **Mobile responsiveness**
  - Use responsive Tailwind classes (`sm:`, `md:`, `lg:`) to adapt:
    - Stack sections vertically on mobile.
    - Keep slides horizontally scrollable or switch to vertical for narrow screens.
    - Ensure enlarged profile picture scales nicely on small devices.
  - Test on different viewport sizes.

---

### Phase 5: Animations & Slide Transitions

- **Horizontal slide behavior**
  - Implement left-to-right transitions between sections using:
    - CSS transforms and transitions, or
    - A small animation library (optional) while keeping Tailwind for styling.
  - Navigation via:
    - Top navigation menu.
    - Next/Previous arrows.
    - Keyboard arrows (optional enhancement).
- **Micro-interactions**
  - Subtle hover on cards and buttons.
  - Smooth scroll for in-page navigation.

---

### Phase 6: Content Integration & Polish

- **Fill with real resume data**
  - Replace placeholders with your actual resume details.
  - Verify spelling, grammar, and consistency.
  - Add external links to GitHub, LinkedIn, and live demos.
- **Accessibility**
  - Use semantic HTML tags.
  - Ensure sufficient color contrast against purple backgrounds.
  - Add alt text for profile picture and images.

---

### Phase 7: Testing

- **Functional testing**
  - Check navigation between all slides.
  - Verify links, buttons, and contact form (if present).
- **Responsive testing**
  - Test on:
    - Small mobile (≤ 375px width),
    - Tablet (768px),
    - Desktop (≥ 1280px).
- **Cross-browser checks**
  - Confirm in at least Chrome, Edge, and Firefox.

---

### Phase 8: Automation & Deployment

- **GitHub setup**
  - Create a new GitHub repository for the project.
  - Commit and push the code to GitHub.
- **Vercel deployment**
  - Connect your GitHub repository to Vercel.
  - Configure build settings (Next.js or static site).
  - Verify automatic deployments on every push to the main branch.
- **CI/CD enhancements (optional)**
  - Add basic checks (linting, tests) that run before deployment.

---

### Phase 9: Maintenance & Iteration

- **Ongoing improvements**
  - Add new projects and experiences as your resume grows.
  - Refine animations and layout based on feedback.
  - Monitor performance and optimize images and assets if needed.

