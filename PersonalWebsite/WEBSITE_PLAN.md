# AI Agent Brief: Mingbo Feng Interactive Personal Website

This document is a handoff brief for building Mingbo Feng's personal GitHub Pages website in a new repository.

The target repository will be:

```text
Mingbaof.github.io
```

The target public URL is:

```text
https://mingbaof.github.io/
```

The new repository is expected to contain at least:

```text
README.md
Resume_MingbaoF.tex
```

The implementing agent should read both files before building the site. `README.md` contains Mingbo's current GitHub profile style, identity, links, and tech stack. `Resume_MingbaoF.tex` contains the formal resume details, work experience, metrics, and project information.

## 1. Core Goal

Build a polished multi-page personal portfolio website for Mingbo Feng.

The website should present Mingbo as a software developer with strong experience in:

- MedTech software reliability.
- FinTech software reliability.
- Software quality assurance.
- Automation tooling.
- CI/CD and release workflows.
- Full-stack web systems.
- Hardware-adjacent software and testing workflows.

The website should be more complete and navigable than the GitHub profile README, but it should preserve the same personal identity: coastal/ocean visual language, clean engineering focus, and approachable professional tone.

The site should not feel like a static PowerPoint or a long resume page. It should have an intentional user flow, interactive navigation, and a memorable pixel-art summer beach experience that leads visitors into Mingbo's about, resume, contact, internship, project, and skill content.

## 2. Important Identity Decisions

Use these decisions as fixed requirements:

- Public English name: `Mingbo Feng`.
- Chinese name: `Mingbao Feng`.
- Primary website display name should be `Mingbo Feng`.
- It is acceptable to mention `Mingbao Feng` as the Chinese name in an understated way, such as in the hero subtitle or about section.
- Location: Edmonton, AB, Canada.
- Hometown/personal identity: Zhuhai, Guangdong, China.
- Education: Bachelor of Science, Honors in Computing Science, University of Alberta.
- Graduation: December 2025, if included.
- Contact email: `mingbao@ualberta.ca`.
- GitHub: `https://github.com/Mingbaof`.
- LinkedIn: `https://www.linkedin.com/in/mingbo-feng-198556257/`.

## 3. Website Scope

Version 1 should be a multi-page website with interactive navigation.

Do not build the site as one long page of stacked text sections. The main page should act as an interactive entry point, while detail pages should give each experience/project room to breathe.

Recommended pages:

1. Home / Interactive Beach.
2. About.
3. Experience detail pages.
4. Project detail pages.
5. Skills / Toolkit.
6. Resume.
7. Contact.

Recommended routes:

```text
/
/about
/experience/software-developer-intern
/experience/software-quality-assurance-intern
/projects/distributed-social-platform
/skills
/resume
/contact
```

Use route names that are stable, readable, and easy to share.

## 4. Positioning and Copy Direction

Suggested headline:

```text
Software Developer building reliable software for MedTech, FinTech, automation, and full-stack systems.
```

Suggested supporting copy:

```text
Computing Science Honors graduate from the University of Alberta with experience across medical imaging software, hardware automation, test infrastructure, CI/CD, and distributed web systems.
```

The content should lean more toward MedTech and FinTech software reliability than generic full-stack development. Full-stack experience should still be included, but it should support the broader reliability/tooling story.

Tone:

- Confident.
- Warm.
- Concrete.
- Professional but not stiff.
- Use metrics from the resume where they strengthen credibility.
- Avoid overclaiming or sounding inflated.

## 5. UI / UX Concept

The website should be built around an interactive summer ocean/beach metaphor inspired by Mingbo's coastal identity from Zhuhai.

### Main Interaction

The home page should feature an interactive pixel-art beach scene. The visual inspiration should be cozy pixel RPG/farming-game art, similar in feeling to Stardew Valley, while using original assets rather than copied game art.

Core idea:

- The entire website should use a pixel-art visual language, not only the beach.
- The overall mood should be summer beach: blue ocean, yellow sunshine, warm sand, clean sky.
- The beach has animated pixel waves.
- The ocean moves through a flood-and-ebb cycle.
- The waves should visibly come toward the shells.
- When the wave layer is on top of the shells, the shells should become hidden or visually submerged.
- When the waves retreat, the shells should appear again on the beach.
- The shells should use actual shell imagery or sprites in the same pixel-art style.
- The main page should stay very clean and should not show many buttons or visible options.
- The primary visible shell set on the main page should be:
  - About Me.
  - Resume.
  - Contact.
- Additional internship/project/skills content can be reached through detail-page links, the sun dropdown, or later expanded shell states if the design remains clean.
- Shells should be visibly interactive through hover/focus states.
- When a user clicks a shell, a shovel animation should dig it up.
- After the shovel animation, the site should navigate to the matching detail page.

### Sun Dropdown Navigation

The sun should act as the compact navigation menu.

Requirements:

- The sun should be visible on the main beach page as part of the pixel-art summer scene.
- The sun should be clickable/tappable.
- Clicking the sun should open a clean dropdown/menu.
- The dropdown should include redirects to:
  - About Me.
  - Resume.
  - Contact.
- The sun menu can also include Experience, Projects, and Skills if needed, but the default should stay minimal.
- The dropdown should feel like part of the pixel-art scene, not like a generic web menu pasted on top.
- The menu must be keyboard accessible and close when the user selects an item, clicks outside, or presses Escape.

This interaction should be central to the experience, not a tiny decorative element.

### Desired Feeling

The user should feel like they are exploring Mingbo's professional story by discovering objects on a beach.

The site should feel:

- Playful, but still professional.
- Interactive, but not confusing.
- Ocean-inspired, but not cartoonish to the point of weakening credibility.
- Technical enough to show craft.
- Calm enough to suit MedTech and FinTech reliability work.

### UX Flow

Recommended flow:

1. Visitor lands on `/`.
2. Visitor sees a clean pixel summer beach scene: ocean waves, sunshine, sand, and a small number of shells.
3. Visitor can click the sun to open a compact dropdown for About Me, Resume, and Contact.
4. Pixel waves roll in and temporarily cover the shells.
5. The waves ebb away and reveal clickable shell sprites on the sand.
6. Visitor hovers or focuses a shell and sees a compact label.
7. Visitor clicks a shell.
8. Shovel animation digs up the shell.
9. Site navigates to the relevant detail page.
10. Detail page presents the selected content with richer explanation, metrics, tech stack, and links where relevant.
11. User can return to the beach or use the sun/menu navigation.

### Navigation Requirements

The beach interaction and sun dropdown should be the primary navigation experience.

Also include:

- Avoid a large conventional header/nav on the main page.
- If a conventional nav is needed on detail pages, keep it compact and secondary.
- Keyboard-accessible shell selection.
- Keyboard-accessible sun dropdown.
- Visible focus states.
- Clear route URLs.
- A way to return to the beach from every detail page.
- A fallback layout for users who cannot or do not want to use the animated pixel beach scene.

### Detail Page UX

Each detail page should feel like opening a discovered shell.

Recommended page structure:

- Back to Beach link.
- Title and role/project name.
- Short summary.
- Timeline/date/location if relevant.
- Tech stack.
- 3 to 5 high-value bullet points.
- Metrics/proof points.
- Related links, if available.
- Next/previous item navigation.

Avoid dumping the entire resume into each page. The detail pages should be curated and readable.

## 6. Pixel-Art Interactive Design Requirements

Use a proven rendering approach rather than hand-rolling complex animation logic.

Recommended options:

- Canvas-based 2D rendering for pixel-art animation.
- Three.js or React Three Fiber only if the implementation uses a 2.5D pixel scene.
- CSS sprite animation is acceptable for simple wave/shell/shovel motion if it remains polished and responsive.

The beach scene does not need photorealistic 3D. It should prioritize a charming pixel-art look with clear interaction. A 2D or 2.5D implementation is preferred if it better serves the Stardew-Valley-like feeling.

Required interactive elements:

- Animated pixel tide or wave movement.
- Waves that travel over the shell positions.
- Shell sprites that become invisible/submerged while waves cover them.
- Shell sprites that reappear when the water retreats.
- Hover/focus state on shells.
- Click/select action on shells.
- Pixel-style shovel/dig animation before navigation.

Performance and usability requirements:

- The scene must load quickly enough for a portfolio site.
- The scene should not block all content if WebGL fails.
- Provide reduced-motion behavior for users who prefer reduced motion.
- Keep labels readable on mobile and desktop.
- Make touch interaction work on mobile.
- Ensure the page still communicates Mingbo's identity before the user interacts.

Visual notes:

- Pixel style is required across the website.
- The beach, waves, sunshine, shells, shovel, labels, menus, and page accents should all feel visually related.
- Shells should look like actual shells, not abstract icons or emoji.
- Create or source original/licensed pixel-art shell assets. Do not copy Stardew Valley assets.
- Use images or generated bitmap-style assets where helpful.
- Avoid relying on emoji as core UI.
- Avoid a wall of plain text on the home page.
- Avoid cluttering the main page with many buttons, panels, badges, or options.
- Do not make the UI feel like a generic template.

## 7. Source Files to Read

Before implementation, read:

```text
README.md
Resume_MingbaoF.tex
```

Use `README.md` for:

- Current visual identity.
- Ocean/coastal theme.
- Social/contact links.
- High-level About Me details.
- Tech stack grouping.
- Existing asset references.

Use `Resume_MingbaoF.tex` for:

- Formal name/contact details.
- Education.
- Work experience.
- Project details.
- Strong metrics and technical keywords.
- Accurate dates and role titles.

## 8. Content Details to Extract

### Hero

Include:

- `Mingbo Feng`.
- Small optional note: `Mingbao Feng`.
- Software Developer / SQA Engineer.
- Edmonton, AB, Canada.
- Short reliability-focused headline.
- Primary actions:
  - Explore the Beach.
  - View Resume.
  - Contact.

The hero should coexist with the interactive beach scene. It should not dominate the whole page as a static text block.

### About

Include:

- BSc Honors in Computing Science from University of Alberta.
- From Zhuhai, Guangdong, China; based in Edmonton, AB.
- Interests and strengths:
  - MedTech software.
  - FinTech software reliability.
  - Hardware automation.
  - Software quality and verification.
  - Full-stack systems.
- A short human paragraph connecting reliability, tools, and user impact.

### Experience

Use the resume as the source of truth.

Include these two roles:

1. Software Developer Intern, Pulse Medica Corp.
   - Dates: Dec. 2024 to Dec. 2025.
   - Location: Edmonton, AB.
   - Tech: Python, Tkinter, TypeScript, React, Redux, Vite, gRPC, C++, GitHub Actions, VirtualBox, FLIR Camera SDK, Zaber Motion Library.
   - Themes: automation tools, hardware integration, installers, CI/CD, UI performance.
   - Suggested shell visual: a polished blue shell with small circuit-like highlights.

2. Software Quality Assurance Intern, Pulse Medica Corp.
   - Dates: May 2024 to Dec. 2024.
   - Location: Edmonton, AB.
   - Tech: Jira, Zephyr Scale, Playwright, TestComplete, HTML/CSS, PowerShell, GitHub, SQL/JQL, OCT, SLO, femtosecond laser systems.
   - Themes: V&V, automated testing, regression efficiency, dashboards, regulatory traceability.
   - Suggested shell visual: a shell with a checkmark/test-grid motif.

Strong proof points to consider:

- Saved 10+ minutes per procedure with 99% accuracy using Python/Tkinter automation tools.
- Reduced repetitive pre-experiment validation time by 83%.
- Built GitHub Actions CI/CD, linting, unit tests, packaging, NSIS installers, and Slack notifications.
- Dependency installer adopted by 3 teams and reduced setup time by 80%.
- Increased automated test coverage from 0% to 30%.
- Reduced regression cycle time from 5 hours to 3 hours.
- Supported V&V across 5 pre-clinical trials.
- Achieved 100% pass rate for release regression with zero critical bugs, according to the resume.

### Projects

At minimum, include:

1. Full-stack Distributed Social Media Platform.
   - Django REST Framework, RESTful API, Python, PostgreSQL, Heroku, pytest, TypeScript, esbuild, OpenAPI/Swagger, Git.
   - Include the YouTube demo link from the resume if present.
   - Emphasize 6-person team leadership, Agile planning, CI/codespaces/branching, authenticated federated nodes, OpenAPI documentation, and 75% propagation-latency improvement.
   - Suggested shell visual: a network-pattern shell or message-in-a-shell object.

Optional later project candidates:

- Dependency installer with React/TypeScript, PowerShell, and Python.
- Hardware automation tool suite.
- Playwright/TestComplete automation framework.
- Android QR-code project if broader student-project coverage is desired.

### Skills

Use these groups unless the source files suggest a better grouping:

- Languages: Python, C++, TypeScript, JavaScript, HTML/CSS, SQL, Java, Kotlin.
- Frontend: React, Redux, Vite.
- Backend: Django, Flask, Node.js, gRPC.
- Testing and QA: Playwright, TestComplete, Zephyr Scale, Jira, JQL/SQL dashboards.
- DevOps and Tools: GitHub Actions, Docker, Linux, PowerShell, VirtualBox, Git.
- Domain: MedTech, medical imaging, hardware automation, regulatory V&V, FinTech reliability.

Suggested interactive representation:

- Skills can be shown as a toolkit or tide map on `/skills`.
- Skill groups should be easy to scan and should not require playful interaction to understand.

### Resume

The source resume file is:

```text
Resume_MingbaoF.tex
```

The resume PDF will be added manually by Mingbo later as a repository asset.

The website should include a resume button/link, but the implementation should tolerate the PDF not existing yet. If a placeholder path is needed, use something simple and easy to replace, such as:

```text
/resume.pdf
```

or:

```text
/assets/Mingbo_Feng_Resume.pdf
```

Make the path easy to update.

The resume page can include:

- Resume download/view button.
- Short note that the PDF asset may be added later.
- Compact summary of Mingbo's profile.
- Link back to the beach.

### Contact

Include:

- Email: `mingbao@ualberta.ca`.
- LinkedIn: `https://www.linkedin.com/in/mingbo-feng-198556257/`.
- GitHub: `https://github.com/Mingbaof`.

The contact copy can invite conversations, collaboration, and opportunities, but should not sound desperate or overly sales-like.

## 9. Visual Direction

Carry forward the current README identity:

- Ocean/coastal theme inspired by Zhuhai.
- Summer beach mood.
- Main colors should emphasize blue and yellow:
  - Blue for ocean, sky, links, and cool accents.
  - Yellow for sun, warm highlights, selected states, and small callouts.
  - Sand/off-white can be used as a neutral base.
- Pixel-art visual language inspired by cozy RPG/farming games, similar in feeling to Stardew Valley.
- Use original pixel assets; do not copy proprietary game sprites.
- Avoid making the entire UI one-note blue; yellow and sand tones should balance the palette.
- Use a clean, technical, calm style.
- Make the site feel suitable for MedTech/FinTech reliability work: polished, readable, trustworthy.
- Avoid a generic marketing landing page feel.
- Avoid oversized decoration that weakens the professional content.
- Avoid plain emoji-based UI.
- Use image, canvas, sprite, or 2.5D elements where they meaningfully support the experience.

If the repo contains existing assets such as:

```text
assets/coding-ocean.png
assets/coding-ocean.svg
```

the implementing agent may use them, especially in the hero or about area. If those assets are not present in the new repo, build the first version without depending on them or add a clear placeholder.

## 10. Recommended Technical Stack

Use:

- Vite.
- React.
- TypeScript.
- React Router.
- Canvas, CSS sprite animation, or React-friendly animation tooling for pixel-art interactions.
- Three.js or React Three Fiber only if the beach is implemented as a 2.5D pixel scene.
- CSS modules, plain CSS, or a lightweight styling approach.

Reasoning:

- It matches Mingbo's current skills.
- It is appropriate for a multi-page interactive portfolio.
- It deploys cleanly to GitHub Pages.
- It supports pixel-art interaction, data files, and project expansion.

Do not over-engineer Version 1, but do implement the beach interaction as the signature experience. The rest of the site can stay simple and readable.

Suggested structure:

```text
.
├── README.md
├── Resume_MingbaoF.tex
├── WEBSITE_PLAN.md
├── package.json
├── index.html
├── vite.config.ts
├── tsconfig.json
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   ├── styles.css
│   ├── data/
│   │   ├── experience.ts
│   │   ├── projects.ts
│   │   ├── shells.ts
│   │   └── skills.ts
│   ├── pages/
│   │   ├── Home.tsx
│   │   ├── About.tsx
│   │   ├── ExperienceDetail.tsx
│   │   ├── ProjectDetail.tsx
│   │   ├── SkillsPage.tsx
│   │   ├── ResumePage.tsx
│   │   └── ContactPage.tsx
│   └── components/
│       ├── Header.tsx
│       ├── BeachScene.tsx
│       ├── WaveLayer.tsx
│       ├── SunMenu.tsx
│       ├── Shell.tsx
│       ├── ShovelAnimation.tsx
│       ├── Section.tsx
│       ├── Experience.tsx
│       ├── Projects.tsx
│       ├── Skills.tsx
│       └── Contact.tsx
└── public/
    └── resume.pdf
```

`public/resume.pdf` is optional until Mingbo adds the real PDF.

## 11. GitHub Pages Deployment Requirements

Because the repository should be named `Mingbaof.github.io`, configure the site for the root Pages URL:

```ts
export default defineConfig({
  base: "/",
  plugins: [react()],
});
```

Add a GitHub Actions workflow for Pages deployment.

Suggested workflow path:

```text
.github/workflows/deploy-pages.yml
```

The workflow should:

- Run on pushes to `main`.
- Install Node dependencies.
- Build the Vite site.
- Upload the `dist` directory as a Pages artifact.
- Deploy to GitHub Pages.

After the workflow is added, GitHub Pages should be enabled in repo settings with source set to GitHub Actions.

Routing note:

- For a multi-page React app on GitHub Pages, use either `HashRouter` or add a proper SPA fallback strategy.
- Prefer clean-looking URLs if feasible, but do not break page refreshes.
- Verify direct navigation to detail pages works after deployment.

## 12. Implementation Milestones

### Milestone 1: Scaffold

- Create the Vite + React + TypeScript app.
- Add React Router.
- Add the chosen rendering/animation approach for the pixel beach.
- Add app shell and global styling.
- Configure Vite base path as `/`.
- Confirm local development works.

### Milestone 2: UX Prototype

- Build a first version of the beach scene.
- Add pixel sun element.
- Add clickable sun dropdown navigation.
- Animate pixel wave movement.
- Make waves travel over shell positions.
- Hide/submerge shells while waves cover them.
- Reveal shells when waves retreat.
- Add actual pixel shell sprites.
- Keep the main page shell set minimal: About Me, Resume, Contact.
- Add shell hover/focus states.
- Add pixel-style shovel animation.
- Connect shell selection to routes.
- Add keyboard and mobile/touch support.

### Milestone 3: Content

- Read `README.md` and `Resume_MingbaoF.tex`.
- Extract content into reusable data files.
- Build home, about, experience detail, project detail, skills, resume, and contact pages.
- Add all contact/project links.

### Milestone 4: Design Polish

- Tune typography, spacing, color, and responsive layout.
- Make the first viewport clearly show Mingbo's identity and reliability-focused positioning.
- Make the beach scene feel like the main UX instead of decoration.
- Keep the main page visually clean: ocean waves, sun, beach, and a small shell set.
- Ensure the sun dropdown replaces the need for many visible buttons.
- Make the whole website feel pixel-styled, including detail pages, buttons, borders, and decorative UI accents.
- Ensure mobile layout is readable.
- Ensure links/buttons are keyboard accessible.
- Add reduced-motion handling.
- Add basic SEO metadata.

### Milestone 5: Deployment

- Add GitHub Actions Pages workflow.
- Run production build.
- Fix build issues.
- Commit implementation.
- Push to `main`.
- Enable GitHub Pages from GitHub Actions.

### Milestone 6: Verification

Verify:

- `https://mingbaof.github.io/` loads after deployment.
- Home beach scene renders correctly.
- Pixel wave animation is visible.
- Sun dropdown opens, closes, and navigates correctly.
- Shells disappear when covered by waves and reappear when waves retreat.
- Shell sprites look like actual shells and match the pixel-art style.
- Shell interactions work with mouse, keyboard, and touch.
- Shovel animation plays before navigation.
- Direct links to detail pages work after refresh.
- Pages, links, and assets render correctly.
- Resume link does not break the page even if the final PDF is not present yet.
- Mobile and desktop layouts are readable.
- WebGL failure or reduced-motion preference does not make the site unusable.
- Page refresh works.
- Lighthouse/accessibility issues are reasonable.

## 13. Open Decisions for Mingbo

Ask Mingbo only if needed. Otherwise make reasonable assumptions and proceed.

Remaining decisions:

1. Which optional projects should appear beyond the distributed social media platform?
2. How close should the site feel to cozy farming/RPG pixel art versus a more modern pixel UI?
3. Should contact copy mention active job search, collaboration, or general contact only?
4. What final file path should the resume PDF use once Mingbo adds it?
5. Should the beach include sound effects, or should it stay silent?
6. Should the main page shells remain only About Me, Resume, and Contact, or later expand to include internships/projects?

Recommended default assumptions:

- Include only the distributed social media platform in Version 1 unless more project details are available.
- Make the ocean theme visually prominent on the home page, and make detail pages professional but still pixel-styled.
- Use blue and yellow as the primary palette, supported by sand/off-white neutrals.
- Keep the main page minimal: waves, sunshine, beach, and three shell links.
- Use general contact/collaboration wording.
- Use `/resume.pdf` as the simplest future resume path.
- Do not include sound in Version 1.

## 14. Final Expected Output

The implementing agent should produce:

- A multi-page Vite + React + TypeScript personal website.
- A pixel-art interactive beach home page.
- A clean summer beach palette centered on blue and yellow.
- Animated pixel wave/flood/ebb behavior.
- Waves that cover shells and make them disappear/submerge.
- Shells that reappear when waves retreat.
- Clickable shell sprites for About Me, Resume, and Contact on the main page.
- A clickable sun dropdown menu linking to About Me, Resume, and Contact.
- Pixel-style shovel animation that plays before navigation.
- Clean responsive UI.
- Content derived from `README.md` and `Resume_MingbaoF.tex`.
- GitHub Pages deployment workflow.
- Root URL configuration for `https://mingbaof.github.io/`.
- A README update if needed explaining local development and deployment.

The website should make Mingbo Feng look credible, technical, and approachable, with a clear emphasis on reliable software for MedTech and FinTech contexts. It should also feel memorable: visitors should discover Mingbo's work through an interactive coastal scene instead of reading a plain resume page.
