# Yasanga P. — Portfolio Website

A responsive, multi-page static portfolio website using HTML, CSS and vanilla JavaScript. It is designed to be easy to host on **GitHub Pages** and simple to update without a build system.

## 1. Preview locally
Open `index.html` in your browser. For a more reliable local preview, use VS Code's **Live Server** extension.

## 2. Add your real portfolio JPG/PNG images
1. Open `assets/projects/`.
2. Copy your project images into that folder. Use simple names such as `flyer-01.jpg`, `brochure-01.jpg`, `onepager-01.jpg`.
3. Open `projects.js`.
4. For each project, change the `image` value to match your file path, for example:
   `image: "assets/projects/flyer-01.jpg"`
5. Change the project title, category, description, overview, objective and creative direction to match the actual project.
6. To add another project, copy one project object in `projects.js`, give it a unique `id`, and update its details.
7. Set `featured: true` for projects you want on the homepage.

Recommended images: JPG or WebP, landscape or portrait according to the artwork, ideally 1400–2000 px on the long edge. Compress large images before uploading. Do not use client work publicly unless you have permission.

## 3. Add your portrait
Place your portrait at `assets/images/portrait.jpg`. In `about.html`, replace the `portrait-placeholder` block with:
```html
<img class="portrait-photo" src="assets/images/portrait.jpg" alt="Yasanga P.">
```
Then add this CSS to `styles.css`:
```css
.portrait-photo { width:100%; height:510px; object-fit:cover; display:block; }
```

## 4. Activate the contact form
The contact form is prepared for **Formspree**:
1. Create a form at https://formspree.io/ and set its recipient to `rasinduy@gmail.com`.
2. Copy the form endpoint ID.
3. In `script.js`, replace `YOUR_FORM_ID` in `https://formspree.io/f/YOUR_FORM_ID` with your real ID.
4. Publish and test the form. Until configured, the page explains that visitors can email you directly.

## 5. Publish with GitHub Pages
1. Sign in to GitHub and create a new public repository, for example `yasanga-portfolio`.
2. Upload all files and folders from this project (keep the folder structure).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. Your site URL will look like `https://YOUR-USERNAME.github.io/yasanga-portfolio/`.

If you want the site at `https://YOUR-USERNAME.github.io/`, name the repository exactly `YOUR-USERNAME.github.io`.

## 6. Important before launch
- Replace all sample portfolio entries and placeholder images. The sample projects are explicitly placeholders, not real client work.
- Add your own LinkedIn profile URL in `contact.html` and `index.html` only when ready.
- Test every page on mobile and desktop.
- Configure Formspree and send a test inquiry.
- Add a custom domain later through GitHub Pages settings if desired.

## Files
- `index.html` — homepage
- `work.html` — filterable portfolio
- `project.html` — reusable individual project detail page
- `services.html` — services
- `about.html` — about and design process
- `contact.html` — contact details and inquiry form
- `projects.js` — edit portfolio projects and image paths
- `styles.css` — visual design and responsive layout
- `script.js` — navigation, portfolio rendering and form behavior
