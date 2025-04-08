# GitHub Contribution Streak Automation

This repository contains a GitHub Actions workflow that automatically maintains your GitHub contribution streak by creating 40-50 commits daily.

## How It Works

The automation:
- Runs daily at midnight UTC
- Creates between 40-50 commits automatically
- Updates a `streak.txt` file with timestamps
- Pushes changes using GitHub Actions bot

## Setup Instructions

1. Fork or clone this repository
2. Ensure GitHub Actions is enabled in your repository settings:
   - Go to Settings > Actions > General
   - Under "Actions permissions", select "Allow all actions and reusable workflows"

## Manual Trigger

You can manually trigger the workflow:
1. Go to the "Actions" tab in your repository
2. Select "Daily Contribution Streak"
3. Click "Run workflow"

## Security Note

This workflow uses the built-in `GITHUB_TOKEN` for authentication, so no additional secrets are required.

## Customization

You can modify `.github/workflows/daily-commits.yml` to:
- Change the schedule (modify the cron expression)
- Adjust the number of commits
- Customize commit messages
- Add more files to update

## Disclaimer

This is for educational purposes only. Please use responsibly and in accordance with GitHub's terms of service. 