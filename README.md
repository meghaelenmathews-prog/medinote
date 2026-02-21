<p align="center">
  <img src="./banner.jpeg" alt="Project Banner" width="100%">
<p align="center">
  <img src="./banner.jpeg" alt="Medinote Banner" style="max-width:100%;height:auto;" />
</p>

# Medinote

An accessible, static web app for quick medicine lookup, interaction alerts, and a guided symptom checker.

- Hosted demo: https://meghaelenmathews-prog.github.io/medinote/

---

## Summary

`Medinote` helps users and caregivers find concise, reliable information about medicines: indications, typical dosages, common side effects, and basic interaction alerts. The project is a mobile-first, static web app built with HTML, CSS, and JavaScript and is optimized for offline caching and simple deployment (GitHub Pages or any static host).

---

## Key Features

- Smart fuzzy search across medicines and indications
- Symptom checker with suggested conditions and next steps
- Drug interaction alerts and contraindication warnings
- Clear dosage guidance and patient-friendly summaries
- Favorites, search history, and export/print summaries
- Offline-first caching of core data and assets
- Responsive, accessible UI (mobile-first)

---

## Tech Stack

- Languages: HTML, CSS, JavaScript
- Storage: local JSON + `localStorage` for user preferences
- Hosting: GitHub Pages (docs/ folder) or any static host
- Dev tools: VS Code, Live Server (for local previews)

---

## Install & Run (local)

1. Clone the repository:

```
git clone https://github.com/<your-username>/medinote.git
cd medinote
```

2. Quick preview: open `index.html` in a browser.

3. Recommended (local server):

Python 3:
```
python -m http.server 8000
# visit http://localhost:8000
```

Node (http-server):
```
npm install -g http-server
http-server -c-1
# visit http://localhost:8080
```

---

## Usage

- Use the search bar to find medicines by name, active ingredient, or indication.
- Open a medicine card to view dosage, interactions, and evidence links.
- Add items to Favorites to save for later; use Export/Print for patient summaries.

---

## Contributing

Contributions are welcome. Please open issues for bugs or feature requests and submit pull requests for code changes. Keep changes focused and include a short description of the change and any testing steps.

Suggested workflow:

1. Fork the repo and create a feature branch.
2. Make changes and add documentation/screenshots where applicable.
3. Open a pull request with a clear description and testing steps.

---

## Project Structure (high level)

- `index.html` — main application UI
- `assets/` — images, icons, screenshots
- `data/` — JSON lists of medicines and metadata
- `docs/` — hosted documentation site (GitHub Pages)

Adjust paths as needed for your repo layout.

---

## License

This project is available under the MIT License. See the `LICENSE` file for details.

---

If you want, I can also:
- expand the `docs/index.html` overview page to match this README,
- generate a CONTRIBUTING.md and CODE_OF_CONDUCT.md,
- add example screenshots and a small changelog.

Made with ❤ by the Medinote team.


