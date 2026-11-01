# Jan Škrabánek | GLOBALMUS Fieldnotes

A Czech-first, bilingual personal journal about Jan Škrabánek's Interreg Volunteer Youth experience with the GLOBALMUS project. The site is static HTML, CSS, and vanilla JavaScript; GitHub Pages serves it directly from the repository root with no build step.

## Publish with GitHub Pages

The existing workflow in `.github/workflows/pages.yml` deploys the site whenever changes are pushed to `main`. Enable **Settings > Pages > Build and deployment > GitHub Actions** in the destination repository.

1. Fork this repository to your GitHub account, or create a new repository under your account. The current `origin` points to the original template repository, so do not push to it.
2. Point `origin` to your fork or new repository and push `main`:

	```sh
	git remote set-url origin https://github.com/<your-username>/<your-repository>.git
	git push -u origin main
	```

3. In your repository, open **Settings > Pages** and set the build and deployment source to **GitHub Actions**.
4. Open the **Actions** tab and wait for **Deploy static site to GitHub Pages** to finish. Your site will be available at `https://<your-username>.github.io/<your-repository>/`.

## Updating content

- Personal photos are stored in `assets/images/my-photos/`: the hero image at the root, the portrait in `portraits/`, and event images in `events/`.
- The About portrait uses a 4:5 crop with `object-fit: cover`. Adjust `object-position` in `assets/css/journal.css` if you want to change the face framing.
- The journal, conference, and fieldwork photo galleries, including Czech/English alt text and undated captions, are maintained in the `galleryGroups` object in `assets/js/journal.js`.
- Event cards and bilingual reports are part of the Events & Activities section in `index.html`. Conference and fieldwork photos are stored in `assets/images/my-photos/events/globalmus-kickoff/` and `assets/images/my-photos/events/fish-sampling/`.
- The About, My Role, Why I Joined, and project sections use the current bilingual site copy. Keep future changes consistent in both languages.

## Verified sources

- [What is Interreg](https://interreg.eu/about/what-is-interreg/)
- [What is Interreg Volunteer Youth](https://www.interregyouth.com/about/what-is-ivy/)
- The GLOBALMUS description and partner details on this site use the information supplied for the website. The project name is kept as GLOBALMUS and is not expanded.

## Credits

The original blog template is by [Coding Stella](https://github.com/codingstella/personal-blog-website). The displayed photographs are copies supplied for this project; source originals were left unchanged.
