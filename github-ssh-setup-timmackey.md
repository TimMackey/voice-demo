# GitHub SSH Setup for TimMackey
**Date:** 2025-05-05

## 🔐 SSH Key Setup

- Private key file: `~/.ssh/id_timmackey_github_key`
- Public key added to GitHub at: https://github.com/settings/keys
- GitHub username: `TimMackey`

## 🛠 SSH Config File (`~/.ssh/config`)

```ssh
Host github-timmackey
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_timmackey_github_key
```

## 🔄 Global Git Setting (optional)

Redirect HTTPS to use SSH:
```bash
git config --global url."git@github-timmackey:".insteadOf "https://github.com/"
```

## ✅ Commands

### Clone a repo

```bash
git clone git@github-timmackey:TimMackey/<repo-name>.git
```

### Push a repo

```bash
git push -u origin main
```

### Force push if needed

```bash
git push -u origin main --force
```

### Test SSH connection

```bash
ssh -T git@github-timmackey
```

Expected output:
```
Hi TimMackey! You've successfully authenticated, but GitHub does not provide shell access.
```

---

## 📁 Notes

- Gradescan projects can continue using HTTPS and credential manager.
- `github-timmackey` ensures Git uses the correct SSH key for TimMackey without interfering with other accounts.

