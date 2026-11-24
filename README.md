# Magic System Wiki

A rune magic system wiki built with Jekyll and the Just the Docs theme, hosted on GitHub Pages. No build workflow is needed; GitHub builds Jekyll itself.

## Publishing

1. Push this repo to GitHub with `README.md` and the `docs/` folder at the top level.
2. Open `docs/_config.yml` and replace `YOUR-USERNAME` and `YOUR-REPO-NAME` (including the `baseurl` line).
3. Go to **Settings → Pages → Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main** (or master), folder: **/docs**
4. Save, wait a minute or two, and the site appears at `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`.

## Adding a page

1. Copy a file from `docs/templates/` into the right folder.
2. Add front matter at the top of the new page:

   ```yaml
   ---
   title: Page Title
   parent: Section Title     # must match the section index page's title exactly
   nav_order: 3              # position in the sidebar
   ---
   ```

3. For a new top-level section, make an `index.md` with `has_children: true`.

Commit, and the sidebar updates automatically.
