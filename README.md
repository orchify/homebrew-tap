# Homebrew Tap for Orchify

Install Orchify CLI:

```bash
brew tap orchify/tap
brew install orchify

Or install directly:

brew install orchify/tap/orchify

Upgrade:

brew update
brew upgrade orchify

Verify:

orchify version

Run a local Orchify runner:

orchify runtime local \
  --api-base-url https://api.orchify.dev \
  --runner-token YOUR_RUNNER_TOKEN \
  --label "$(hostname)"

Run as a background service:

export ORCHIFY_API_BASE_URL=https://api.orchify.dev
export ORCHIFY_RUNNER_TOKEN=YOUR_RUNNER_TOKEN
brew services start orchify
