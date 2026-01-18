# Folder Usage Guide - orbios-kb-board

Quick reference guide for when to use each folder in the board repository.

## Quick Decision Tree

```
Is it strategic/board-level? 
├─ NO → Use orbios-kb-core or orbios-kb-public
└─ YES → Continue...

What type of content?
├─ Static knowledge/documentation → context/
│   ├─ Company strategy → context/company/
│   ├─ Financial planning → context/finances/
│   ├─ Org structure → context/organization/
│   └─ Coordination → context/coordination/
│
├─ Review/evaluation → reviews/
│
├─ Update/status report → updates/
│
├─ Mission/TF-mission → missions/
│
└─ Services/data → services/
    ├─ Financial tracking → services/finances/
    └─ Service notes → services/notes/
```

## Detailed Folder Usage

### 📁 `context/` - Static Knowledge (Board Level)

**When to use**: Strategic knowledge and reference documentation at board level.

**Subfolders**:

| Folder | Use When | Example |
|--------|----------|---------|
| `company/` | Company strategy, board decisions, long-term goals | `company/strategic-plan-2026.md` |
| `finances/` | High-level financial planning, cross-cluster coordination | `finances/annual-projection-2026.md` |
| `organization/` | Top-level org structure, executive roles | `organization/executive-org-chart.md` |
| `coordination/` | Inter-cluster coordination, responsibility distribution | `coordination/cross-cluster-initiatives.md` |

**❌ Don't use for**: Cluster-level details, operational specifics

---

### 📁 `reviews/` - Board-Level Reviews

**When to use**: Strategic reviews, performance evaluations, decision reviews.

**Format**: `YYYY-MM-DD_review_type_subject.md`

**Examples**:
- `2026-01-15_strategic_review_q1-2026.md`
- `2026-01-20_performance_review_team-leads.md`

**❌ Don't use for**: Operational reviews (use core repo)

---

### 📁 `updates/` - Board-Level Updates

**When to use**: Strategic updates, key metrics, decisions needed from board.

**Format**: `YYYY-MM-DD_update_type.md`

**Examples**:
- `2026-01-15_strategic_update.md`
- `2026-01-20_financial_update.md`
- `2026-01-25_decision_request.md`

**❌ Don't use for**: Operational updates (use core repo)

---

### 📁 `missions/` - TF-Missions (Board Level)

**When to use**: Strategic task force missions requiring cross-functional coordination.

**Format**: `mission-name/` (directory with mission files)

**Examples**:
- `missions/strategic-initiative-2026/`
- `missions/cross-cluster-coordination/`

**❌ Don't use for**: Operational missions (use core repo)

---

### 📁 `services/` - Services and Data (Board Level)

**When to use**: Company services, subscriptions, financial data at board level.

**Subfolders**:

| Folder | Use When | Example |
|--------|----------|---------|
| `finances/` | Financial tracking, current month, annual projection | `finances/current-month.md` |
| `finances/history/` | Historical financial data | `finances/history/2026-01.md` |
| `notes/` | Service documentation, configuration | `notes/google-workspace.md` |
| `services.yaml` | Single source of truth for all services | `services/services.yaml` |

**❌ Don't use for**: Cluster-level service details

---

## Common Scenarios

### Scenario 1: Strategic Decision

**Question**: Where to document a strategic board decision?

**Answer**: 
- Decision document → `context/company/decision-name.md`
- Review → `reviews/YYYY-MM-DD_decision_review_topic.md`
- Update → `updates/YYYY-MM-DD_strategic_update.md`

---

### Scenario 2: Financial Planning

**Question**: Where to store financial projections and budgets?

**Answer**:
- Strategic financial planning → `context/finances/annual-projection-2026.md`
- Current month tracking → `services/finances/current-month.md`
- Historical data → `services/finances/history/YYYY-MM.md`

---

### Scenario 3: Service Management

**Question**: Where to document company services and subscriptions?

**Answer**:
- Service data → `services/services.yaml` (single source of truth)
- Service notes → `services/notes/service-name.md`
- Financial tracking → `services/finances/current-month.md`

---

### Scenario 4: Cross-Cluster Coordination

**Question**: Where to document coordination between clusters?

**Answer**:
- Coordination docs → `context/coordination/initiative-name.md`
- Mission → `missions/cross-cluster-mission-name/`
- Update → `updates/YYYY-MM-DD_coordination_update.md`

---

## Security Checklist

Before creating a document, verify:

- [ ] Content is strategic/board-level (not operational)
- [ ] No cluster-level details (use appropriate repo)
- [ ] Appropriate folder selected
- [ ] Template used (if available)
- [ ] Document name follows convention
- [ ] Content is in English
- [ ] Strategic information is properly marked

---

## Related Guides

- Main README: [`README.md`](README.md)
- Core Repository Guide: [`orbios-kb-core/FOLDER-USAGE-GUIDE.md`](https://github.com/Orbios/orbios-kb-core)
- Public Repository Guide: [`orbios-kb-public/README.md`](https://github.com/Orbios/orbios-kb-public)

---

**Last Updated**: 2026-01-06

