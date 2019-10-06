# git-commit-formatter
Individual repository to improve the quality of Git Commit Message

# Setting up in Local Project
1. Go to the root directory of your project.

2. Download the pre-commit-msg file into the `.git/hooks/` directory. Give Executable permission to the file

```bash
wget https://raw.githubusercontent.com/AdityaSidharta/git-commit-formatter/master/prepare-commit-msg -O .git/hooks/prepare-commit-msg
chmod +x .git/hooks/prepare-commit-msg
```

# Setting up Globally

1. Set up Git template for all new projects
```bash
cd 
git config --global init.templatedir '~/.git-templates'
mkdir -p ~/.git-templates/hooks
wget https://raw.githubusercontent.com/AdityaSidharta/git-commit-formatter/master/prepare-commit-msg -O ~/.git-templates/hooks/prepare-commit-msg
chmod +x ~/.git-templates/hooks/prepare-commit-msg
```

2. Initialize Git for new projects.
```bash
git init
```
