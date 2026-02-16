# 💼 Gig Economy Scraper & Review Workflow

A GitHub-based workflow for tracking and reviewing gig economy opportunities.

## 🎯 Purpose

This repository manages Jad's gig hunting workflow:
1. **Scraper** auto-creates issues for new opportunities
2. **Project Board** tracks review state
3. **Issue Templates** standardize gig documentation

## 📋 Project Board

Track gigs through the review process: [Projects → Gig Review Workflow](https://github.com/atEverychance/gig-economy/projects)

**Columns:**
- 📥 **Incoming** - New gigs found by scraper
- 👀 **Reviewing** - Gigs being evaluated
- ✅ **Applied** - Applications submitted
- ❌ **Rejected** - Passed on opportunities

## 🏗️ Setup Instructions

### 1. Create the Project Board (Manual)

1. Go to [github.com/atEverychance/gig-economy/projects](https://github.com/atEverychance/gig-economy/projects)
2. Click "New project" → "Classic project"
3. Name: **Gig Review Workflow**
4. Add columns in order:
   - Incoming
   - Reviewing
   - Applied
   - Rejected

### 2. Issue Templates

Two templates are available when creating issues:

| Template | Use For | Created By |
|----------|---------|------------|
| 🤖 **New Gig Found** | Auto-generated gig alerts | Scraper bot |
| 📝 **Gig Review Notes** | Manual review documentation | Jad |

## 🔌 Scraper Integration

See [docs/SCRAPER.md](docs/SCRAPER.md) for:
- API endpoints and commands
- Issue creation format
- Rate limiting guidance
- Testing procedures

## 🏷️ Labels

| Label | Purpose |
|-------|---------|
| `new-gig` | Fresh opportunities from scraper |
| `incoming` | In the "Incoming" column |
| `review-notes` | Manual review documentation |

## 🚀 Quick Commands

```bash
# List recent gigs
gh issue list --repo atEverychance/gig-economy --label "new-gig"

# View project board
gh project view --owner atEverychance --project "Gig Review Workflow"
```

## 📝 Workflow

1. **Scraper finds gig** → Creates issue → Auto-adds to "Incoming"
2. **Jad reviews** → Moves to "Reviewing" → Optionally creates review notes
3. **Decision made** → Move to "Applied" or "Rejected"

---

*Generated for OpenClaw agent workspace*
