# Tratonomous Rebranding Summary

## Overview

This document summarizes the comprehensive rebranding of the application from **OpenAlgo** to **Tratonomous**.

**Date:** January 28, 2026  
**Repository:** https://github.com/tratonomous-crypto/tratonomous  
**License:** AGPL-3.0  
**Upstream:** https://github.com/marketcalls/openalgo

---

## AGPL-3.0 Compliance ✅

As a fork of [OpenAlgo](https://github.com/marketcalls/openalgo), Tratonomous fully complies with AGPL-3.0:

| Requirement | Status | Implementation |
|-------------|--------|----------------|
| License File | ✅ | `license.txt` with full AGPL-3.0 text |
| Fork Attribution | ✅ | README.md has prominent fork notice |
| Original Copyright | ✅ | Original authors (marketcalls) credited |
| Modification Notice | ✅ | README clearly states modified version |
| Same License | ✅ | Project remains AGPL-3.0 |
| Source Code Access | ✅ | Public GitHub repo linked in UI |

---

## What Was Rebranded

### UI & Frontend
| Item | Before | After |
|------|--------|-------|
| Page Title | OpenAlgo | Tratonomous |
| Meta Description | OpenAlgo Platform | Tratonomous Platform |
| Navbar Brand | openalgo | tratonomous |
| Footer Brand | OpenAlgo | Tratonomous |
| GitHub Links | marketcalls/openalgo | tratonomous-crypto/tratonomous |

### Environment Variables
| Before | After |
|--------|-------|
| `OPENALGO_API_KEY` | `TRATONOMOUS_API_KEY` |

### Type Definitions
| Before | After |
|--------|-------|
| `openalgo_username` | `tratonomous_username` |
| `openalgo_host` | `tratonomous_host` |
| `openalgo_ws_url` | `tratonomous_ws_url` |

### Local Storage Keys
| Before | After |
|--------|-------|
| `openalgo_positions_prefs` | `tratonomous_positions_prefs` |

---

## What Was Preserved

These were **intentionally NOT changed** (external resources/SDK):

- `https://docs.openalgo.in` - Upstream documentation site
- `pip install openalgo` - SDK package name  
- `from openalgo import api` - SDK import
- OpenAlgo community links (Discord, Twitter, YouTube)

---

## Files Modified

### Root Level
- `README.md` - Complete rebrand with AGPL-3.0 attribution
- `license.txt` - Full AGPL-3.0 license text
- `REBRANDING_SUMMARY.md` - This file

### Frontend Components
- `Navbar.tsx` - Brand name, logo
- `Footer.tsx` - Brand labels, GitHub link
- `navigation.ts` - Docs link label

### Frontend Pages
- `Home.tsx`, `Login.tsx`, `Faq.tsx`, `Dashboard.tsx`
- `Playground.tsx`, `Positions.tsx`, `FlowEditor.tsx`
- `PythonStrategyGuide.tsx`, `NewPythonStrategy.tsx`
- `TelegramUsers.tsx`, `TelegramAnalytics.tsx`

### Type Definitions
- `telegram.ts`, `flow.ts`

### HTML
- `index.html` - Title, meta description

### Documentation
- `frontend/docs/frontend/README.md`
- `frontend/docs/frontend/developer-guide.md`
- `frontend/docs/frontend/testing-guide.md`
- `frontend/docs/frontend/components.md`
- `frontend/docs/frontend/api-reference.md`
- `gocharting_webhook_setup.md`

---

## Git Commits

| Commit | Description |
|--------|-------------|
| `e3962460` | Frontend rebrand: all UI brand names, types, env vars |
| `caf08fcf` | Update GitHub links to tratonomous-crypto |
| `25238b9e` | AGPL-3.0 license + README attribution |

---

## Verification Checklist

- [x] No "OpenAlgo" (PascalCase) in source code
- [x] All "openalgo" lowercase = external links or SDK only
- [x] GitHub links point to new repository
- [x] Frontend builds successfully
- [x] UI displays "Tratonomous" branding
- [x] AGPL-3.0 license file included
- [x] README has fork attribution
- [x] Pushed to GitHub successfully

---

## Build Commands

```bash
cd frontend
npm install
npm run build
```

---

**Status: COMPLETE** ✅

Pushed to: https://github.com/tratonomous-crypto/tratonomous
