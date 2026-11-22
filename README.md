# Magic System Wiki

Source for a MkDocs Material wiki documenting my magic system, published with GitHub Pages.

## Local preview

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve        # http://127.0.0.1:8000
```

## Publishing

1. Create a GitHub repo and push this folder to the `main` branch.
2. Edit `site_url` and `repo_url` in `mkdocs.yml` with your username and repo name.
3. After the first workflow run, go to **Settings → Pages**, set the source to **Deploy from a branch**, and choose `gh-pages` / `(root)`.
4. The site appears at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

## Adding content

- Copy a file from `docs/templates/` into the right folder.
- Add the page to the `nav:` section in `mkdocs.yml`.
- Push to `main`; the site rebuilds automatically.
