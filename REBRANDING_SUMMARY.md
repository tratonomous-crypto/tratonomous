# Tratonomous Frontend Rebranding Summary

## Overview

This document summarizes the comprehensive rebranding of the frontend application from **OpenAlgo** to **Tratonomous**.

**Date:** January 28, 2026  
**Repository:** https://github.com/tratonomous-crypto/tratonomous  
**License:** AGPL-3.0

---

## AGPL-3.0 Compliance

As a fork of [OpenAlgo](https://github.com/marketcalls/openalgo), Tratonomous complies with AGPL-3.0 requirements:

| Requirement | Implementation |
|-------------|----------------|
| **License File** | ✅ `license.txt` - Full AGPL-3.0 text included |
| **Fork Attribution** | ✅ README.md includes prominent fork notice |
| **Original Copyright** | ✅ Original authors credited in README |
| **Modification Notice** | ✅ README clearly states this is a modified version |
| **Same License** | ✅ Project remains AGPL-3.0 licensed |
| **Source Code Access** | ✅ Public GitHub repo with source link in UI |

## Rebranding Rules Applied

### Renamed
| Original | New |
|----------|-----|
| `OpenAlgo` (PascalCase) | `Tratonomous` |
| `openalgo` (lowercase brand references) | `tratonomous` |
| `OPENALGO_API_KEY` | `TRATONOMOUS_API_KEY` |
| `openalgo_username` | `tratonomous_username` |
| `openalgo_host` | `tratonomous_host` |
| `openalgo_ws_url` | `tratonomous_ws_url` |
| `openalgo_positions_prefs` | `tratonomous_positions_prefs` |

### Preserved (External Links & SDK)
These were intentionally **NOT** changed as they refer to external resources or the SDK package:

- `https://docs.openalgo.in` - External documentation site
- `pip install openalgo` - SDK package name
- `from openalgo import api` - SDK import statement
- `openalgo/pyproject.toml` - SDK file path references
- `openalgo/requirements.txt` - SDK file path references

### Updated GitHub Links
| Original | New |
|----------|-----|
| `github.com/marketcalls/openalgo` | `github.com/tratonomous-crypto/tratonomous` |

---

## Files Modified

### Core UI Components

| File | Changes |
|------|---------|
| `frontend/src/components/layout/Navbar.tsx` | Brand name in header, logo alt text |
| `frontend/src/components/layout/Footer.tsx` | Brand name labels, GitHub link |
| `frontend/src/config/navigation.ts` | Docs navigation label |

### Pages

| File | Changes |
|------|---------|
| `frontend/src/pages/Home.tsx` | Brand name in mobile menu and header |
| `frontend/src/pages/Login.tsx` | GitHub link |
| `frontend/src/pages/Faq.tsx` | GitHub help section link |
| `frontend/src/pages/Dashboard.tsx` | Quick access card labels |
| `frontend/src/pages/Playground.tsx` | Header brand text |
| `frontend/src/pages/Positions.tsx` | Local storage key |
| `frontend/src/pages/flow/FlowEditor.tsx` | Header brand text |
| `frontend/src/pages/python-strategy/PythonStrategyGuide.tsx` | SDK references, env variable names |
| `frontend/src/pages/python-strategy/NewPythonStrategy.tsx` | Example strategy comments, env variable |
| `frontend/src/pages/telegram/TelegramUsers.tsx` | Username field references |
| `frontend/src/pages/telegram/TelegramAnalytics.tsx` | Username field references |

### Type Definitions

| File | Changes |
|------|---------|
| `frontend/src/types/telegram.ts` | `openalgo_username` → `tratonomous_username` |
| `frontend/src/types/flow.ts` | `openalgo_host` → `tratonomous_host`, `openalgo_ws_url` → `tratonomous_ws_url` |

### HTML & Configuration

| File | Changes |
|------|---------|
| `frontend/index.html` | Page title, meta description |

### Documentation

| File | Changes |
|------|---------|
| `frontend/docs/frontend/README.md` | Title and introduction |
| `frontend/docs/frontend/developer-guide.md` | Introduction text |
| `frontend/docs/frontend/testing-guide.md` | Introduction text |
| `frontend/docs/frontend/components.md` | Introduction text |
| `frontend/docs/frontend/api-reference.md` | Introduction text |
| `frontend/public/docs/gocharting_webhook_setup.md` | All brand references, GitHub links |

---

## Build & Deployment

The frontend was rebuilt after all source changes:

```bash
cd frontend
npm install
npm run build
```

The `dist/` folder now contains the production bundle with all Tratonomous branding.

---

## Git Commits

1. **`e3962460`** - `refactor(frontend): complete rebrand from OpenAlgo to Tratonomous`
   - All UI brand name updates
   - Type definitions and environment variables
   - Frontend documentation
   - Rebuilt frontend dist bundle

2. **`caf08fcf`** - `chore: update GitHub repo links to tratonomous-crypto/tratonomous per AGPL-3.0`
   - Updated all GitHub repository references
   - Footer, Login, FAQ pages
   - Documentation files

---

## Verification

After deployment, verified:
- ✅ No "OpenAlgo" (PascalCase) references remain in source
- ✅ All "openalgo" (lowercase) references are preserved external links or SDK references
- ✅ GitHub links point to new repository
- ✅ Frontend builds successfully
- ✅ UI displays "Tratonomous" branding

---

## Notes

- **AGPL-3.0 Compliance**: The source code link in the UI now points to the new public repository
- **External Documentation**: Links to `docs.openalgo.in` are preserved as the documentation site remains external
- **SDK Package**: The Python SDK package name (`openalgo`) is preserved as it's a separate package
