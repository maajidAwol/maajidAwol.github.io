# Abdulmajid Awol Seid

Source for my academic website: **[maajidawol.github.io](https://maajidawol.github.io/)**

I am a PhD student in Computer Science at [Tulane University](https://sse.tulane.edu/cs) and a graduate research assistant in the [Laboratory for Software Design](https://lab-design.github.io/). I research reliable and secure AI agents at the intersection of artificial intelligence, software engineering, and programming languages.

- **Research:** [maajidawol.github.io/research](https://maajidawol.github.io/research/)
- **CV:** [maajidawol.github.io/cv](https://maajidawol.github.io/cv/)
- **Email:** [aseid@tulane.edu](mailto:aseid@tulane.edu)

## How this site is built

The site is built with [Jekyll](https://jekyllrb.com/) using the [al-folio](https://github.com/alshedivat/al-folio) starter (MIT License). Pushing to `main` runs the `Deploy site` GitHub Actions workflow, which builds the site and publishes it to the `gh-pages` branch served by GitHub Pages.

Where the content lives:

| Content        | File(s)                                  |
| -------------- | ---------------------------------------- |
| Homepage       | `_pages/about.md`                        |
| Research       | `_pages/research.md`                     |
| About          | `_pages/about-me.md`                     |
| Projects       | `_projects/`                             |
| Publications   | `_bibliography/papers.bib`               |
| CV page        | `_data/cv.yml`                           |
| CV PDF         | `assets/pdf/Abdulmajid_Awol_Seid_CV.pdf` |
| CV PDF source  | `assets/rendercv/academic_cv.yaml`       |
| News           | `_news/`                                 |
| Research notes | `_posts/`                                |
| Site settings  | `_config.yml`, `_data/socials.yml`       |

To regenerate the CV PDF after editing `assets/rendercv/academic_cv.yaml`:

```bash
uv tool run --python 3.12 --from "rendercv[full]" rendercv render assets/rendercv/academic_cv.yaml
```
