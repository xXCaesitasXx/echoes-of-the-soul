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
3. Go to **Settings → Pages → Build and deployment** and set Source to **GitHub Actions**. Do this *before* or right after your first push.
4. Open the **Actions** tab. The "Deploy wiki" run should turn green (use **Run workflow** to trigger it manually if needed).
5. The site appears at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

If the front page shows only the README, Pages is still set to "Deploy from a branch" instead of "GitHub Actions".

## Adding content

- Copy a file from `docs/templates/` into the right folder.
- Add the page to the `nav:` section in `mkdocs.yml`.
- Push to `main`; the site rebuilds automatically.
