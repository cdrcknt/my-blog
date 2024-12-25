---
title: "Git Workflow Basics: A Student's Guide to Version Control"
description: "Master the essential Git commands and workflows that every computer science student needs to know for effective project management."
pubDate: 2024-03-10
image: "https://images.unsplash.com/photo-1618401471353-b98afee0b2eb?w=800&auto=format&fit=crop&q=80"
tags: ["Git", "Version Control", "Tutorial", "Programming"]
---

Git is an essential tool for every developer. Let's explore the basic commands and workflows you'll use daily.

## Getting Started

Initialize a new repository and make your first commit:

```bash
# Initialize a new repository
git init

# Add files to staging
git add index.html

# Commit changes
git commit -m "Initial commit"
```

## Basic Workflow Commands

### Checking Status and History

```bash
# Check repository status
git status

# View commit history
git log
```

### Working with Branches

```bash
# Create and switch to a new branch
git checkout -b feature/login

# Switch between branches
git checkout main

# Merge branches
git merge feature/login
```

## Best Practices

1. **Commit Messages**
   - Write clear, descriptive messages
   - Use present tense
   - Keep it concise but informative

2. **Branching Strategy**
   - main/master: stable production code
   - develop: integration branch
   - feature/: new features
   - bugfix/: bug fixes

3. **Regular Updates**
   ```bash
   # Update your local repository
   git pull origin main

   # Push your changes
   git push origin feature/login
   ```

## Common Scenarios

### Fixing Mistakes

```bash
# Undo last commit (keeping changes)
git reset --soft HEAD~1

# Discard changes in working directory
git checkout -- file.txt

# Amend last commit
git commit --amend
```

### Collaboration

```bash
# Clone a repository
git clone https://github.com/username/repo.git

# Create a pull request
# 1. Push your branch
git push origin feature/login

# 2. Visit the repository on GitHub
# 3. Click "New Pull Request"
```

Remember to commit often and keep your commits atomic (one logical change per commit). This makes it easier to track changes and fix issues when they arise.

Stay tuned for more programming and development tips!