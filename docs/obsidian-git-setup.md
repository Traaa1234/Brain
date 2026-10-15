# Sync Obsidian to this repo with the Obsidian Git plugin

## 1. One-time: get the repo on your computer
Install Git (https://git-scm.com), then:

    git clone https://github.com/Traaa1234/brain.git

GitHub no longer accepts account passwords for git. Sign in with either:
- **GitHub Desktop** or **Git Credential Manager** (a browser login pops up), or
- a **Personal Access Token**: GitHub > Settings > Developer settings > Fine-grained tokens >
  repository access: `brain` only, permission **Contents: Read and write**.
  Use the token as the password when git asks.

## 2. Point Obsidian at the vault folder
- Obsidian > "Open folder as vault" > choose `brain/obsidian/vault`
- Already have a vault? Copy its files into `brain/obsidian/vault/` first, then open that folder.

## 3. Install the plugin
1. Settings > Community plugins > **Turn on community plugins**
2. **Browse** > search **Obsidian Git** (by Vinzent03) > **Install** > **Enable**

## 4. Recommended plugin settings (Settings > Obsidian Git)
- **Auto commit-and-sync interval (minutes):** 10
- **Auto pull interval (minutes):** 10
- **Pull on startup:** on
- **Commit message:** `vault backup: {{date}}`
- **Sync method:** Merge (default) is fine

Manual use: Command palette (Ctrl/Cmd+P) > "Obsidian Git: Commit-and-sync".

## 5. Mobile (optional)
Obsidian Git is experimental on iOS/Android and slow on large vaults. For phones,
use Obsidian Sync, or only pull on mobile.

## Notes
- Keep the repo private.
- `.gitignore` already skips `workspace.json` so layout changes don't cause conflicts.
- Don't edit the same note on two devices before they've synced.
