# Paua Market Planner (family copy)

A read-only, password-protected copy of the family's paua board: product ideas, business plans,
research and next steps for each market. The live, editable board stays on claude.ai.

- `board.html.enc` is the board, encrypted so its content isn't readable in this public repository.
- `.github/workflows/deploy.yml` unlocks it, locks the page with the family password, and publishes it
  to GitHub Pages on every push to `main`.

Repository secrets (Settings > Secrets and variables > Actions):

- `PAGE_PASSWORD`: the password the family types to open the page.
- `SOURCE_KEY`: the key that unlocks `board.html.enc`.

To change the family password, update `PAGE_PASSWORD`, then open the Actions tab and run
"Publish password-protected board" again.
