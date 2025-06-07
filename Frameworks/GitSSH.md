# Quick Command Reference

---

## 1. GIT SSH Setup

### Single Account
```bash
# Generate SSH key
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

# Start ssh-agent and add key
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa

# Copy SSH key for GitHub/GitLab
cat ~/.ssh/id_rsa.pub

# Test connection
ssh -T git@github.com
```
### Multiple accounts
# Generate separate keys
```
ssh-keygen -t rsa -b 4096 -C "work_email@example.com" -f ~/.ssh/id_rsa_work

ssh-keygen -t rsa -b 4096 -C "personal_email@example.com" -f ~/.ssh/id_rsa_personal
```

# ~/.ssh/config example
```
Host github-work
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa_work

Host github-personal
    HostName github.com
    User git
    IdentityFile ~/.ssh/id_rsa_personal
```
# Clone repos using hosts aliases
```
git clone git@github-work:username/repo.git
git clone git@github-personal:username/repo.git
```



