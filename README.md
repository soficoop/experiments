# Experiments Collection

A collection of interactive experiments, simulations, games, and tools built with HTML, CSS, and JavaScript.

## 🎯 Available Experiments

- **Percolation Simulation** - Interactive visualization of percolation theory
- **Yield Calculator** - Financial tool for calculating investment yields
- **CSV Diff Validator** - Compare and validate differences between CSV files
- **Pong Game** - Classic Pong game implementation
- **CSV → MSSQL Generator** - Generate T-SQL UPDATE statements from CSV files

## 🌿 Branch Deployments

This repository uses GitHub Pages with automatic branch deployments. Each branch is automatically deployed when code is pushed:

- **Main branch**: Deployed to the root URL
- **Feature branches**: Deployed to `/branches/{branch-name}/`
- **Develop branch**: Deployed to `/branches/develop/`

### How it works

1. When you push to any tracked branch (`main`, `develop`, `feature/**`, `hotfix/**`), GitHub Actions automatically deploys it
2. The main branch is always deployed to the root of the site
3. Other branches are deployed to subdirectories under `/branches/`
4. A branch index page at `/branches/` lists all available branch deployments
5. The main site includes a link to view all branch deployments

### Accessing Branch Deployments

- Main site: `https://soficoop.github.io/experiments/`
- Branch deployments: `https://soficoop.github.io/experiments/branches/`
- Specific branch: `https://soficoop.github.io/experiments/branches/{branch-name}/`

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
3. Push the branch - it will be automatically deployed for testing
4. Create a pull request to merge into main

The branch deployment system allows you to test your changes live before merging!