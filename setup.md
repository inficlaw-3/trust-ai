# Setup

> Start your journey here. Each step introduces new trust assumptions — they'll be called out explicitly.

---

## Step 1: Clone to Your Personal Account

Fork or clone this repository to your own GitHub account. **Keep it private.**

This repository is your **master control plane**. Everything flows from here:
- All secrets will be configured in this repo
- All infrastructure deployment will be coordinated through this repo
- All agent behavior is defined by the code here

### Branch Protection

After cloning, set up branch protection on `main`:
- Require pull request reviews before merging
- Require review from the account owner (you)
- No direct pushes to main

This ensures no code enters your agent without your explicit review.

### New Trust Assumption: Repository Updates

By hosting your own copy, you need to trust that updates to your repository are **only controlled by you**.

This means trusting:

1. **GitHub as a company** — that they don't get hacked and don't work against you
2. **Your own account and credentials** — that they don't get compromised

### How to Clone

```bash
# Clone and push to your own new private repo
git clone https://github.com/infiloop2/trusted-agent.git
cd trusted-agent
git remote set-url origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

Then in GitHub Settings → Branches → Add branch protection rule for `main`.

### Verification

Before proceeding, confirm:
- [ ] You have your own private copy of this repo
- [ ] Branch protection requires your review for all changes
- [ ] You understand this repo is your master control plane
- [ ] You understand the trust assumption above

---

## Step 2: ...

*Coming soon*
