# WhatsApp Media Bot (Baileys prototype)

## What's included
- Node.js + Baileys-based prototype
- Auto-save media from groups/chats into `downloads/`
- Admin commands: setforward / stopforward / kick
- Simple DB (db.json) with media index & user upload counts
- Menu and basic download command

## Setup (quick)
1. Ensure Node 16+ installed.
2. Unzip project and `cd wa-media-bot`.
3. Copy `.env.example` to `.env` and set `OWNER` to your phone (947... without +).
4. Install deps:
   ```bash
   npm install
   ```
5. Start the bot:
   ```bash
   node index.js
   ```
6. A QR code will show in the terminal. Scan it from WhatsApp (Linked devices -> Link a device) to attach the account.
7. Invite that account to groups or send media to it — media will be saved to `downloads/` and logged in `db.json`.

## Notes & production
- This is an unofficial method (uses WhatsApp Web reverse-engineered protocol). For production, prefer WhatsApp Cloud API (official).
- Be mindful of privacy & consent when saving others' media.
- The `OWNER` number controls owner-only commands. Use your full number like `9477XXXXXXX`.

