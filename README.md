# Connected by Design — Lakshmana Kontemukkula

A responsive personal portfolio homepage built with **vanilla HTML5, CSS3, and ES6+**. The site presents my background, selected projects, and an interactive Project Explorer without using a front-end framework or component library.

## Author

**[Lakshmana Kontemukkula — portfolio homepage](./index.html)**  
MS in Computer Science, Northeastern University · Expected May 2027

[LinkedIn](https://linkedin.com/in/lakshmana-k-785727291) · [Email](mailto:lakshmana.2003k@gmail.com) · [Résumé PDF](./docs/lakshmana-resume.pdf)

## Class Link

Replace this before submission with the official course/Canvas link:

`PASTE_CLASS_LINK_HERE`

## Project Objective

The goal of this project is to create a meaningful public homepage that introduces who I am, demonstrates my technical interests, and gives visitors an easy way to explore representative work. The implementation uses semantic HTML, organized CSS, and native ES6 modules.

## Live Site

After GitHub Pages deployment, replace this with the public URL:

`PASTE_GITHUB_PAGES_URL_HERE`

## Screenshot

![Homepage screenshot](./images/homepage-screenshot.png)

## Features

- Responsive homepage with meaningful biography and project content
- Original **Project Explorer** that filters projects by category and updates an `aria-live` summary
- Original **Project Spotlight** interaction written in vanilla JavaScript
- Scroll-reveal interaction using `IntersectionObserver`
- Responsive mobile navigation
- Separate project case-study page
- Résumé-backed education, three internships, skills, LinkedIn/email contact, and a downloadable résumé
- Eight filterable projects, including traffic-control reinforcement learning, water/food monitoring, and an NLP recommender
- Third AI-assisted concept page with an interactive energy-to-task selector
- Editorial typography, local PNG illustrations, project jump links, and illustrated project cards
- Navigation and core content remain usable without JavaScript; reduced motion is respected
- Semantic HTML, keyboard-focusable controls, alt text, and a skip link
- No jQuery, Bootstrap, React, or other UI/component library

## Pages

- `index.html` — main portfolio homepage
- `projects.html` — project case studies
- `ai-lab.html` — AI-assisted third page / concept prototype

## Project Structure

```text
homepage_assignment/
├── index.html                  # Homepage, experience, education, project explorer
├── projects.html               # Eight case studies
├── ai-lab.html                 # AI-generated FocusFlow concept
├── css/styles.css              # Shared responsive design
├── js/main.js                  # Original and enhanced ES6 interactions
├── images/                     # Local PNG art, screenshots, six wireframes
├── docs/
│   ├── design-document.md      # Description, personas, user stories, wireframes
│   ├── rubric-audit.md         # Requirement-by-requirement evidence
│   ├── validation-report.md    # Results and limitations
│   ├── submission-checklist.md
│   ├── video-script.md
│   └── lakshmana-resume.pdf    # Original supplied résumé
├── .gitignore
├── .prettierignore
├── .prettierrc
├── eslint.config.js            # Professor's exact original file
├── package.json
├── LICENSE
└── README.md
```

## Technical Requirements

- A modern browser with JavaScript modules, CSS Grid, and Flexbox support.
- A local HTTP server (VS Code Live Server or Python 3's built-in server).
- Node.js and npm for the declared Prettier/ESLint development tools. The website itself needs neither Node nor a backend once served.
- No build pipeline, API keys, external fonts, runtime packages, or component libraries.
- Development dependencies are listed in `package.json`. Do not replace the professor's `eslint.config.js`.

## Instructions to Build / Run

1. Install a current Node.js version.
2. Open the project folder in VS Code.
3. Run `npm install` in the VS Code terminal.
4. Run `npm run format` to apply Prettier.
5. Run `npm run format:check` to verify formatting.
6. Run `npm run lint` to run the class ESLint configuration.
7. Open `index.html` with the VS Code **Live Server** extension.

### Use the site

1. Open the homepage, browse experience and education, or download the résumé.
2. In Project Explorer, select All, IoT, Machine Learning, or Web to filter eight projects.
3. Follow a case-study link, or use the project index on the Projects page.
4. Select “Show another project” to cycle through the original four Spotlight lessons.
5. Open AI Lab and choose an energy level to highlight a matching sample task.
6. On a phone, use Menu; with a keyboard, use Tab, Enter/Space, and Escape. A skip link leads to the main content.

For a Python server, run `python -m http.server 8000` from this folder and open
[the local homepage](http://localhost:8000). No compilation is needed.

## Formatting and Validation

- Format: `npm run format`
- Check formatting: `npm run format:check`
- JavaScript lint: `npm run lint`
- HTML validation: check `index.html`, `projects.html`, and `ai-lab.html` using the W3C validator before final submission.

## ESLint

This project uses the **class-provided `eslint.config.js`**. It includes the ESLint recommended rules, browser/Node/ES2025 globals, two-space indentation, Unix line endings, double quotes, semicolons, and Prettier integration.

## Creative / Original Component

The homepage includes an original **Project Explorer** written in ES6+. Visitors can choose All, IoT, Machine Learning, or Web. JavaScript reads each project's `data-category`, hides non-matching cards, tracks how many projects remain visible, changes the active filter, and updates an `aria-live` summary.

A second interaction called **Project Spotlight** cycles through project lessons without reloading the page.

## Redesign and Verification

The September 24 redesign and September 25 résumé update preserve all three page URLs and the original project descriptions,
category filtering, Spotlight lessons, scroll reveals, module loading, folder organization,
and the MIT license. The original class ESLint configuration is byte-for-byte unchanged.
The shared design now uses warm paper surfaces, forest green accents, serif highlights,
illustrated project cards, and consistent navigation. FocusFlow adds a local energy selector
using sample tasks; it has no AI service, backend, saved state, or external runtime library.

See [validation results](./docs/validation-report.md) and the
[submission checklist](./docs/submission-checklist.md). Deployment, course/video links,
the required code review, and Google Form submission still require student completion.
No build step is needed: serve this folder using Live Server or `python -m http.server 8000`.
Use an HTTP server so ES6 modules load correctly; opening files directly is not recommended.

## GenAI Use

The original project README records ChatGPT (**GPT-5.6 Sol, September 2026**) as its development assistant. This historical model detail is retained from the supplied project and should be verified against the original conversation before submission. The original work used it to brainstorm the website structure, get help organizing the HTML/CSS files, improve some JavaScript functionality, and review the project against the assignment rubric.

Example prompts included:

- “Help me plan a personal homepage using HTML, CSS, and ES6 modules.”
- “Suggest an original JavaScript feature for my portfolio.”
- “Check whether my project satisfies this assignment rubric.”
- “Help me organize my README and design document.”

The original README states that the student reviewed, edited, and tested the initial generated suggestions. The new redesign also needs a final student review before submission.

The third page, `ai-lab.html`, is intentionally documented as the AI-assisted page. Generative AI was used to help brainstorm its FocusFlow concept, content hierarchy, and initial wording before I reviewed and integrated it into the project.

### September 2026 redesign assistance

- Tool/model: OpenAI Codex, GPT-6 (September 24, 2026). The exact model build identifier is not exposed in this session.
- Inputs: the existing project ZIP, assignment rubric, and the redesign request below.
- Representative user prompt: “Improve the existing homepage assignment website substantially while preserving every rubric requirement and the professor’s exact ESLint config. Make the three pages more polished, modern, cohesive, and professional; keep it vanilla HTML5/CSS3/ES6 modules, static frontend only, no libraries.”
- AI work: revised shared CSS and page layouts, created the local workspace SVG diagram, recolored existing illustrations, improved navigation/filter accessibility, added FocusFlow’s energy selector, updated documents/mockups, and ran browser, formatting, lint, and HTML checks.
- Original project claims were preserved. The September 25 update uses the supplied résumé for additional education, employment, project, and contact details; these are user-provided claims, not independently verified results.
- The student should review the generated code, confirm personal content, understand the interactions, and complete the remaining submission steps. No student review of this revision is claimed yet.
- All three pages received AI-assisted revisions; `ai-lab.html` remains the explicitly designated AI-generated third page.

### September 25 résumé and rubric update

- Tool/model: OpenAI Codex, GPT-6; exact build identifier unavailable.
- User prompt: “Make the assignment better and add if something is missing.”
- Inputs: the supplied résumé PDF and two professor screenshots covering README and design-document expectations, alongside the earlier full rubric.
- Assistance: incorporated résumé content, added four projects and new local SVG illustrations, updated email/LinkedIn links, included the original résumé download, expanded README instructions, created wireframes for every page, and added a rubric-to-evidence map.
- Original four projects absent from the new résumé were retained from the existing assignment. Their accuracy should be confirmed by the student. No repository or public demo links were invented.
- The traffic-control result is explicitly limited to its simulator and 20 evaluation episodes; team attribution is retained. FocusFlow is still a sample-data concept, not an AI-powered service.

### FocusFlow content revision

The optional on-page AI/human contribution cards were replaced with three practical study steps: check in, make it specific, and pause and reset. The AI-assisted page label and this required GenAI disclosure remain. Prompt: “Can you replace this part with something else, only if the assignment allows it.” Codex (GPT-6, exact build unavailable) drafted the replacement copy.

## Deployment

Recommended: GitHub Pages.

1. Push this project to a GitHub repository.
2. Open **Settings → Pages** in the repository.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)` folder.
5. Save and open the public GitHub Pages URL after deployment.
6. Add that URL to this README and to the course submission form.

## Video Demo

A narration script is included at `docs/video-script.md`. Record a short public or unlisted demo showing the homepage, Project Explorer, responsive layout, project page, and AI-assisted third page.

Replace this before submission:

`PASTE_PUBLIC_VIDEO_URL_HERE`

## Documentation

- [Rubric-to-evidence map and remaining requirements](./docs/rubric-audit.md)
- [Design document: personas, stories, decisions, and mockups](./docs/design-document.md)
- [Validation report](./docs/validation-report.md)
- [Narrated demo script](./docs/video-script.md)
- [Remaining submission checklist](./docs/submission-checklist.md)

## License

This project is licensed under the MIT License. See `LICENSE`.

## Image formats

All illustrations, wireframes, and the favicon are supplied as PNG files. Existing artwork was converted from SVG without redesigning it. This changes the file format, not the AI-assistance history described above. Original SVG source files are not included in the submission ZIP.
