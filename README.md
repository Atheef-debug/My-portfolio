# Mohamed Atheef Udayar — Portfolio

Static portfolio website (HTML, CSS, JavaScript). No build step, no dependencies.

## Structure
```
index.html          page markup
css/styles.css      all styling (dark + light themes)
js/config.js        YOUR DETAILS: contact info, skills, projects, experience, education, CV path
js/main.js          rendering, theme toggle, form, animations
assets/images/profile.jpg   profile photo
assets/cv/          put your CV PDF here
.nojekyll, netlify.toml     hosting helpers
```

## Run locally
1. Unzip the folder.
2. Easiest: double-click `index.html`.
3. Or run a local server from the folder: `python3 -m http.server 8000` then open http://localhost:8000
   (or `npx serve .` if you have Node.js).

## Add your CV
1. Copy your PDF into `assets/cv/` (e.g. `ATHEEF-CV.pdf`).
2. In `js/config.js` set `cv:"assets/cv/ATHEEF-CV.pdf"`.

## Add real project links
In `js/config.js`, fill `src:""` (source code) and `demo:""` (live demo) for a project. The buttons appear only when a URL is set. Use only verified URLs.

## Contact form
There is no backend. The form opens the visitor's email app with the message filled in. For real submissions, connect a service such as Formspree or EmailJS.

## Deploy
**GitHub Pages:** create a repository, upload all files (keep the folder structure), then Settings -> Pages -> Deploy from branch -> `main` / root. Site URL: `https://<username>.github.io/<repo>/`.
**Netlify:** drag the folder onto app.netlify.com/drop, or connect the GitHub repo (publish directory `.`).
**Vercel:** import the GitHub repo; framework preset "Other", no build command.
