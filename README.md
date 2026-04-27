# Build Slides Repository

A centralized repository for storing and managing presentation slides for build reviews, planning sessions, and technical discussions.

## Directory Structure

```
.
├── README.md
└── build03/                        # Slides for Build 03
    ├── lody@Leon.key               # source file@author
    └── videcoding@hawkingrei.pptx  # source file@author
```

## Naming Convention

Folders are named by build number: `build<N>`. Files follow the pattern `<topic>@<author>.<ext>` for easy identification.

Examples:
- `build01/`
- `build02/`
- `build03/`

## File Formats

| Format | Purpose |
|--------|---------|
| `.key` | Keynote source file, editable on macOS |
| `.pdf` | Final version for distribution and consistent rendering |

## Usage Guidelines

1. **Create a new folder** per build using the `build<N>` naming convention
2. **Name files** using the `<topic>@<author>.<ext>` pattern
3. **Export to PDF** before committing to ensure consistent rendering across platforms
4. **Compress images** before adding to keep repository size manageable (< 50MB per file)

## Quick Start

```bash
# Create a directory for a new build
mkdir build04
cd build04

# Add your slides
# e.g. cp /path/to/your.pptx mytopic@yourname.pptx

# Commit and push
git add .
git commit -m "Add slides for build04"
git push
```

---

*For questions or template requests, please open an issue or contact the build team.*
