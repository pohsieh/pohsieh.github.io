# pohsieh.github.io

Portfolio site of Po-Yu Hsieh, built with Jekyll and hosted on GitHub Pages. GitHub builds
the site automatically on every push.

## Where the content lives

| What | File |
|---|---|
| One project | `_projects/<name>.md` — settings at the top (between `---`), text below |
| Intro, discipline chain, links | `_data/profile.yml` |
| Publications | `_data/publications.yml` |
| CV | `_data/cv.yml` |
| Images | `assets/img/` |
| Look and feel (colours, fonts, spacing) | `assets/style.css` (tokens at the top) |
| Page templates | `_layouts/` — normally no need to touch |

## Editing

**In the browser (Pages CMS):** go to <https://app.pagescms.org>, sign in with GitHub, pick this
repository. Projects, Profile, Publications and CV appear as forms; images can be uploaded
there. Every save is a commit, and the live site updates a minute later.

**On the computer:** edit the files above, then commit and push.

- **Replace an image:** overwrite the file in `assets/img/` with the same name. With a
  different name or extension, update the path in the project file.
- **Add a project:** copy an existing file in `_projects/`, rename it, and edit it. `order`
  sets its position on the home page and the Previous / Next links. The home page card is
  created automatically.
- **Figures:** `size: full` fills the row; two consecutive `size: half` figures sit side by side.
- Recommended images: long edge 1800–2400 px, under ~500 KB (WebP or JPG).

## Local preview

```bash
/opt/miniconda3/bin/conda run -n jekyll jekyll serve
```

Then open <http://localhost:4000>.
