# Homebrew Tap for Orchify

Install the Orchify CLI:

```bash
brew tap orchify/tap
brew install orchify/tap/orchify
```

Or, if the tap is already added:

```bash
brew install orchify
```

Upgrade:

```bash
brew update
brew upgrade orchify
```

Verify the installation:

```bash
orchify version
```

Run a local Orchify runner:

```bash
orchify runtime local \
  --api-base-url https://api.orchify.dev \
  --runner-token YOUR_RUNNER_TOKEN \
  --label "$(hostname)"
```

Run Orchify as a background service:

```bash
export ORCHIFY_API_BASE_URL=https://api.orchify.dev
export ORCHIFY_RUNNER_TOKEN=YOUR_RUNNER_TOKEN
brew services start orchify
```

Stop the service:

```bash
brew services stop orchify
```
