Astro Portfolio Starter (Khoa Vu–inspired layout)
=================================================

Structure:
- `/`      : Fullscreen landing page with background placeholder and "Enter" link.
- `/works` : Project index (image tiles + footnote-style info).
- `/about` : Bio / CV page.
- `/projects/intergenerational-incubator` : Sample project detail page.

How to use
----------

1. Install Node.js (LTS) from https://nodejs.org if you have not done so.
   You should be able to run `node -v` and `npm -v` in your terminal.

2. In VS Code:
   - Open this folder.
   - Open a terminal at the project root.

3. Install dependencies:

   npm install

4. Run the dev server:

   npm run dev

5. Open the URL shown in the terminal, usually:

   http://localhost:4321/

6. Editing content:

   - Replace "YOUR NAME" with your name in:
       - src/components/Header.astro
       - src/pages/index.astro
       - src/pages/about.astro
   - Update the `works` array in src/pages/works.astro with your own projects.
   - For each project, create a file under src/pages/projects/<slug>.astro
     by copying the sample project file.

7. Replacing images:

   - Export your drawings / renders as JPG/PNG.
   - Put them into the `public` folder, for example:
       public/images/incubator/axon.jpg
   - Replace the placeholder `div` blocks in project pages with `<img>` tags such as:
       <img src="/images/incubator/axon.jpg" alt="Axonometric view" style="width:100%;height:auto;" />

8. Building for deployment:

   npm run build

   The static site will be generated into the `dist` folder.
