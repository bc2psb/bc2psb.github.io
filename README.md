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

## Publishing

The site is live at https://bc2psb.github.io/, built from the `main` branch of
[bc2psb/bc2psb.github.io](https://github.com/bc2psb/bc2psb.github.io) (Settings → Pages).
To give a colleague edit access, add them to the `bc2psb` organization on GitHub.

## Page layout

- `index.html`: the single page, which reads everything from `_data/`
- `_layouts/default.html`: the header, navigation and footer
