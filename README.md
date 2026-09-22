# BC² website

The website of BC² (Behavior, Cognition & Complexity) at Paris School of Business. It runs on GitHub Pages with Jekyll, so there's nothing to install and GitHub rebuilds the site about a minute after every commit.

## Editing content

All content is in `_data/`. You can edit the files directly on github.com (open the file, click the pencil icon, then commit).

| To change…                     | Edit                      |
|--------------------------------|---------------------------|
| Intro, goal, micro/meso/macro  | `_data/about.yml`         |
| Members                        | `_data/members.yml`       |
| External affiliates            | `_data/affiliates.yml`    |
| Activities                     | `_data/activities.yml`    |
| Funded projects                | `_data/projects.yml`      |
| Site title, contact email      | `_config.yml`             |
| Colors and fonts               | `assets/css/style.css`    |

To add a member, copy an existing block in `members.yml` and change it. To add a photo, upload it to `assets/img/` and add `photo: filename.jpg` to that person's block.

YAML tip: keep the indentation exactly as it is in the surrounding entries (spaces, not tabs). If a line contains a colon followed by a space (`: `), wrap the text in quotes.

## Publishing (one-time setup)

1. Create a GitHub repository named `bc2` and upload these files.
2. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, then choose `main` and `/ (root)`.
3. The site appears at `https://<account>.github.io/bc2/`.

## Page layout

- `index.html`: the single page, which reads everything from `_data/`
- `_layouts/default.html`: the header, navigation and footer
