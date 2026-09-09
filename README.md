# MM AI/dev compute expense dashboard (Allied reimbursement tooling)

Unlisted static dashboard. No PHI. Medical category shown as **Private (redacted)**.

**Live:** https://cyberbuilder000.github.io/mm-ai-exp-k7q2/

## Refresh after accruals
```bash
cd /workspace/expense-allocation
python3 tracker.py accrue          # or: dashboard
# then republish index.html from dashboard.html (see below)
```

## Redeploy to GitHub Pages
```bash
cp /workspace/expense-allocation/dashboard.html /path/to/mm-ai-exp-k7q2/index.html
cd /path/to/mm-ai-exp-k7q2
git add index.html && git commit -m "refresh dashboard" && git push
```
