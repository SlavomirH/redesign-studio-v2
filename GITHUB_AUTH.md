# GitHub Auth — Quick Start

To host the site on GitHub, you need a one-time Personal Access Token.

## Steps

1. Open your browser to: **https://github.com/settings/tokens**
2. Click the button: **"Generate new token (classic)"** (NOT fine-grained)
3. In the "Note" field, type: `redesign-studio-deploy`
4. Under "Select scopes", check ONLY: **repo** (full control of private repositories)
5. Click the green **"Generate token"** button at the bottom
6. GitHub shows your new token — it starts with `ghp_...`
7. **COPY it immediately** (you won't see it again)

## What to do next

Once you have the token, come back here and paste it in the chat, or run this in your terminal:

```bash
echo "ghp_YOUR_TOKEN_HERE" | gh auth login --with-token
```

Then I'll create the repo and push everything.

## Why this works

The `gh auth login --web` flow uses a browser redirect that isn't landing in your session. The `--with-token` approach pipes the token directly — no browser needed, no redirect, no timeout.

## Security note

This token gives full access to your repos. I use it once to create `redesign-studio-v2` and push the code, then it's discarded. You can delete the token after deployment from https://github.com/settings/tokens.
