# Experiments Collection

A collection of interactive experiments, simulations, games, and tools built with HTML, CSS, and JavaScript.

## 🎯 Available Experiments

- **Percolation Simulation** - Interactive visualization of percolation theory
- **Yield Calculator** - Financial tool for calculating investment yields
- **CSV Diff Validator** - Compare and validate differences between CSV files
- **Pong Game** - Classic Pong game implementation
- **CSV → MSSQL Generator** - Generate T-SQL UPDATE statements from CSV files

## 🔄 PR Deployments

This repository uses GitHub Pages with automatic pull request deployments. Each pull request is automatically deployed when opened or updated:

- **Main branch**: Deployed to the root URL
- **Pull requests**: Deployed to `/pr/{pr-number}/`

### How it works

1. When you open or update a pull request, GitHub Actions automatically deploys it
2. The main branch is always deployed to the root of the site
3. Pull requests are deployed to subdirectories under `/pr/`
4. A PR index page at `/pr/` lists all available PR deployments
5. The main site includes a link to view all PR deployments
6. When a PR is closed or merged, its deployment is automatically cleaned up

### Accessing PR Deployments

- Main site: `https://soficoop.github.io/experiments/`
- PR deployments: `https://soficoop.github.io/experiments/pr/`
- Specific PR: `https://soficoop.github.io/experiments/pr/{pr-number}/`

## 🚀 Local Development

Since these are static HTML files, you can simply open them in a web browser or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 📁 Project Structure

```
.
├── index.html              # Main landing page
├── percolation.html        # Percolation simulation
├── yield.html             # Yield calculator
├── csv-compare.html       # CSV diff validator
├── pong.html              # Pong game
├── csv-mssql.html         # CSV to MSSQL generator
└── .github/
    └── workflows/
        └── deploy-pages.yml   # GitHub Pages deployment workflow
```

## 🛠️ Adding New Experiments

1. Create a new HTML file in the root directory
2. Add a link to it in `index.html`
3. Commit and push - it will be automatically deployed!

## 📝 Contributing

1. Create a feature branch: `git checkout -b feature/my-new-experiment`
2. Add your experiment
3. Open a pull request - it will be automatically deployed for testing
4. Review your changes at the PR deployment URL
5. Merge the pull request when ready

The PR deployment system allows you to test your changes live before merging!