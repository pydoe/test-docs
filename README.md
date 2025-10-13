# pyDOE3 MkDocs Documentation

This directory contains the MkDocs version of the pyDOE3 documentation, migrated from Sphinx.

## Quick Start

### Prerequisites
- Python 3.8+
- `uv` package manager (recommended) or `pip`

### Setup
1. Create and activate virtual environment:
```bash
uv venv mkdocs-env
source mkdocs-env/bin/activate  # On Windows: mkdocs-env\Scripts\activate
```

2. Install dependencies:
```bash
uv pip install mkdocs mkdocs-material pymdown-extensions mkdocs-minify-plugin
```

### Development
Start the local development server:
```bash
mkdocs serve
```

The documentation will be available at `http://127.0.0.1:8000`

### Build
Generate static site:
```bash
mkdocs build
```

Output will be in the `site/` directory.

## Configuration
The main configuration is in `mkdocs.yml`. Key features:
- **Theme**: Material Design with dark/light mode
- **Search**: Built-in search with highlighting  
- **Math**: MathJax support for mathematical formulas
- **Code**: Syntax highlighting with copy buttons
- **Navigation**: Responsive with tabs and sections

## Content Structure
- `docs/index.md` - Main landing page
- `docs/factorial.md` - Factorial designs (complete)
- `docs/rsm.md` - Response surface designs (complete)
- `docs/randomized.md` - Randomized designs (partial)
- `docs/low_discrepancy_sequences.md` - Low-discrepancy sequences (stub)
- `docs/sampling_designs.md` - Sampling designs (stub)
- `docs/taguchi.md` - Taguchi designs (stub)
- `docs/doe_optimal.md` - Optimal designs (stub)

## Migration Status
✅ Core structure and configuration complete  
✅ Main content pages converted from RST to Markdown  
⚠️ Some sections need full conversion (see MIGRATION_REPORT.md)  

## Development Notes
- All images and static assets are in `docs/assets/`
- Custom styling in `docs/assets/stylesheets/extra.css`
- MathJax configuration in `docs/javascripts/mathjax.js`
- Original Sphinx files remain in `../doc/` for reference

See `../MIGRATION_REPORT.md` for detailed migration information.