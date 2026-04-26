# Build Slides Repository

A centralized repository for storing and managing presentation slides for build reviews, planning sessions, and technical discussions.

## Overview

This repository serves as the single source of truth for all build-related presentations, ensuring easy access, version control, and collaborative editing of slide decks.

## Directory Structure

```
.
├── README.md
├── YYYY-MM-DD-topic/           # Date-prefixed folder for each presentation
│   ├── slides.pdf              # Final exported slides (PDF format)
│   ├── slides.pptx             # Editable source file (optional)
│   ├── assets/                 # Images, diagrams, and supporting files
│   └── notes.md                # Speaker notes or additional context
└── templates/                  # Reusable slide templates
    ├── build-review-template.pptx
    └── planning-template.pptx
```

## Naming Convention

Folders should follow the pattern: `YYYY-MM-DD-<topic>`

Examples:
- `2026-04-26-q2-build-review/`
- `2026-05-15-performance-optimization/`

## File Formats

| Format | Purpose |
|--------|---------|
| `.pdf` | Final version for distribution and archiving |
| `.pptx` | Editable source (include if future edits are likely) |
| `.md` | Speaker notes, summaries, or supplementary documentation |

## Usage Guidelines

1. **Create a new folder** for each presentation using the naming convention
2. **Export to PDF** before committing to ensure consistent rendering
3. **Include speaker notes** in `notes.md` for context and key talking points
4. **Compress images** before adding to keep repository size manageable

## Quick Start

```bash
# Create a new presentation folder
mkdir YYYY-MM-DD-your-topic
cd YYYY-MM-DD-your-topic

# Add your slides and notes
cp ../templates/build-review-template.pptx slides.pptx
# ... edit your slides ...

# Export to PDF and commit
git add .
git commit -m "Add slides for YYYY-MM-DD build review"
git push
```

## Contributing

1. Ensure all slides are properly named and organized
2. Include a brief summary in the folder's `notes.md`
3. Keep individual files under 50MB when possible

---

*For questions or template requests, please open an issue or contact the build team.*
