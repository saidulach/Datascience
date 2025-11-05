🧰 Git Setup & Workflow Cheat Sheet (.md version)

This Markdown guide walks through setting up Git and pushing code to GitHub using SSH, with comments for clarity. You can save this as git_setup_cheat_sheet.md.

---

🔧 Initial Git Setup

# Set your Git username
git config --global user.name "Your Name"

# Set your Git email
git config --global user.email "your.email@example.com"

---

🔐 SSH Key Setup (One-time)

# Generate SSH key
ssh-keygen -t ed25519 -C "your.email@example.com"

# Start SSH agent
eval "$(ssh-agent -s)"

# Add your SSH key to the agent
ssh-add ~/.ssh/id_ed25519

---

📁 Initialize Local Repository

# Create and navigate to your project folder
mkdir my-project
cd my-project

# Initialize Git
git init

---

🌐 Connect to GitHub Repository

# Add remote origin using SSH
git remote add origin git@github.com:your-username/your-repo.git

---

📦 Stage and Commit Changes

# Stage all changes
git add .

# Commit with a message
git commit -m "Initial commit"

---

🚀 Push to GitHub

# Push to the remote repository
git push -u origin master

---

✅ Common Git Commands

# Check status of files
git status

# View commit history
git log

# Clone a repo
git clone git@github.com:user/repo.git

# Pull latest changes
git pull origin main

# Create a new branch
git checkout -b feature-branch
