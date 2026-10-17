# Limane Mohammed | Cybersecurity Portfolio

A personal portfolio website for Limane Mohammed, a cybersecurity student at HIST in Algeria. It is a static site built with plain HTML, CSS, and JavaScript, so it can be hosted for free on GitHub Pages. No build tools, frameworks, or backend are needed.

- GitHub: https://github.com/mohquor
- LinkedIn: https://www.linkedin.com/in/limane-mohammed-9545a043a
- Expected live URL: https://mohquor.github.io/limane-mohammed-portfolioo/

## Project structure

```
limane-mohammed-portfolioo/
├── index.html          Page content and structure
├── style.css           Design system and styling
├── script.js           Mobile menu, scroll effects, hero animation
├── README.md           This guide
└── assets/
    └── favicon.svg     "LM" browser tab icon
```

All paths are relative (for example `style.css`, `assets/favicon.svg`), so the site works under a GitHub Pages project URL.

## Deploy to GitHub Pages (beginner guide)

1. **Create a repository.** Sign in to GitHub, click **New repository**, and name it exactly `limane-mohammed-portfolioo`. Keep it **Public**.
2. **Upload the files.** On the new repository page, click **uploading an existing file**. Drag in `index.html`, `style.css`, `script.js`, `README.md`, and the `assets` folder (with `favicon.svg` inside). The files must sit in the repository root, not inside an extra folder. Click **Commit changes**.
3. **Open Settings.** In your repository, click the **Settings** tab.
4. **Open Pages.** In the left sidebar, click **Pages**.
5. **Choose the source.** Under **Build and deployment**, set **Source** to **Deploy from a branch**.
6. **Pick the branch.** Select the **main** branch and the **/ (root)** folder.
7. **Save.** Click **Save**.
8. **Wait for publishing.** GitHub builds the site. This usually takes 1 to 3 minutes. Refresh the Pages settings screen to see the status.
9. **Open your site.** When it is ready, GitHub shows your link:

   `https://mohquor.github.io/limane-mohammed-portfolioo/`

## Updating the website later

**In the browser:** open the file in your repository, click the pencil icon, edit, and click **Commit changes**. To add a new file, use **Add file > Upload files**.

**With Git on your computer:**

```bash
git add .
git commit -m "Update portfolio"
git push
```

GitHub Pages republishes automatically within a few minutes.

## How to customize

All comments in the code that start with "HOW TO" explain each change.

- **Add or remove a skill:** in `index.html`, copy or delete a line like
  `<li class="skill"><span>Linux Fundamentals</span><span class="tag tag--practicing">Practicing</span></li>`.
  Labels: `tag--foundations`, `tag--learning`, `tag--practicing`, `tag--exploring`.
- **Add a project repository link:** only when the repository really exists, replace the "Documentation Coming Soon" note in that project card with a GitHub button (an example is in the comments inside the Projects section).
- **Add a real certificate:** replace the "Not yet" empty-state box in the Certifications section with a card containing only real details (an example is in the comments).
- **TryHackMe section:** the profile card is in `index.html` under `id="tryhackme"`. Only add rank, points, or badges there if they are your real numbers.
- **Add an email address:** uncomment the example email button in the Contact section and put in your real address.
- **Change colors:** edit the variables at the top of `style.css` (`--green`, `--cyan`, `--bg`, and others).

## Troubleshooting

**The site shows a 404 page or "There isn't a GitHub Pages site here"**
Make sure a file named exactly `index.html` (all lowercase) is in the repository root, not inside a subfolder. Check that Pages is set to the `main` branch and `/ (root)` folder.

**The page appears with no styling (CSS not loading)**
Confirm `style.css` is in the same folder as `index.html` and the name matches exactly. File names are case-sensitive on GitHub Pages, so `Style.css` is not the same as `style.css`. Do a hard refresh (Ctrl+Shift+R, or Cmd+Shift+R on Mac).

**Menu, animations, or the terminal do not work (JavaScript not working)**
Confirm `script.js` is uploaded next to `index.html`. Open your browser's developer tools (F12), go to **Console**, and look for red error messages. A missing file shows up as a 404 in the **Network** tab.

**Icons, the favicon, or other assets are missing (incorrect paths)**
Use relative paths such as `assets/favicon.svg`. Do not start paths with a slash, because `/style.css` points to `mohquor.github.io/style.css` instead of your project folder. Keep the `assets` folder name in lowercase.

**I changed something but the site looks the same (deployment delays)**
Publishing can take a few minutes. Check the **Actions** tab for a running "pages build and deployment" job, wait until it shows a green check, then hard refresh. Browsers sometimes cache old files too.

## Ethical use

This is a portfolio, not a hacking tool. The terminal on the home page is decorative and does not run commands or scan anything.

All security research and testing should be performed only on systems you own or have explicit authorization to test.
