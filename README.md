<div align="center">
  <h1> Daily Commit 📅 </h1>

  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge" />
  <img src="https://img.shields.io/badge/YAML-CB171E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Utility-Automation-blue?style=for-the-badge" />
</div>

## 📌 Overview

**Daily Commit** is a GitHub Actions automation that ensures a commit is made to the repository every day, helping maintain a consistent contribution streak on GitHub.

## 🎯 Objectives

- Automate daily commits to keep the contribution graph active.
- Leverage GitHub Actions scheduled workflows for zero-touch operation.

## 🛠 Features

- **Scheduled Execution**: Runs daily at midnight UTC via cron (`0 0 * * *`).
- **Automatic Logging**: Writes the current date to 'daily_commit.txt' with each commit.
- **Zero Configuration**: Deploy and forget - no local setup required.

## 📂 Project Structure

```text
.
├── .github/
│   └── workflows/
│       └── daily_commit.yml      # GitHub Actions workflow
├── daily_commit.txt              # Daily updating file
└── README.md                     # Project documentation
```

## 🚀 Working

1. **Scheduled Trigger**  
   The workflow is triggered automatically at midnight UTC via a cron schedule.

2. **Checkout Repository**  
   The latest code is checked out using [`actions/checkout@v4`](.github/workflows/daily_commit.yml#L11).

3. **Update daily_commit.txt**  
   The current date and time are written to [`daily_commit.txt`](daily_commit.txt).

4. **Push Chnages**  
   The changes are committed and pushed back to the repository with the timestamp as the commit message.

## ⚙️ Installation & Usage

### 1 Clone the repository

[![Git](https://img.shields.io/badge/Git-F05032?style=plastic)](https://git-scm.com/downloads)
[![Project](https://img.shields.io/badge/Project-Repository-blue?style=plastic)](https://github.com/akshatjasrotia85/daily-commit)

```bash
git clone https://github.com/akshatjasrotia85/daily-commit.git
cd daily-commit
```

### 2 Required Setup

1. **Add your GitHub username and email** in `.github/workflows/daily_commit.yml`:
   ```bash
   git config user.name "your-username"
   git config user.email "your-email@example.com"
   ```
2. **Give Read and Write permissions** in the repository settings:
   - Go to **Settings** → **Actions** → **General**.
   - Under **Workflow permissions**, select **Read and write permissions**.
   - Click **Save**.

## 👤 Author

[![Email](https://img.shields.io/badge/Email-D14836?style=plastic)](mailto:akshatjasrotia85@gmail.com)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=plastic)](https://youtube.com/@akshatjasrotia85)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=plastic)](https://instagram.com/akshatjasrotia85)
[![X](https://img.shields.io/badge/X-000000?style=plastic)](https://x.com/akshatj85)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=plastic)](https://linkedin.com/in/akshat-jasrotia-6b4445418)
[![Unstop](https://img.shields.io/badge/Unstop-1C4980?style=plastic)](https://unstop.com/u/skenatwz97640)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=plastic)](https://leetcode.com/u/akshatjasrotia85/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=plastic)](https://github.com/akshatjasrotia85)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=plastic)](https://hub.docker.com/u/akshatj85)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF6B35?style=plastic)](https://akshatjasrotia85.github.io/akshatjasrotia85/)
