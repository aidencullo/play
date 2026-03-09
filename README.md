# Claude PR Review Demo

A sample repo demonstrating automatic Claude code review on pull requests.

## How it works

Every PR triggers a GitHub Actions workflow that:
1. Gets the PR diff
2. Sends it to Claude (claude-sonnet-4-6) via the Anthropic API
3. Posts the review as a PR comment

## Setup

1. Add your Anthropic API key as a repository secret: `ANTHROPIC_API_KEY`
2. Open a PR — Claude will automatically review it

## Workflow

See [`.github/workflows/claude-review.yml`](.github/workflows/claude-review.yml)
