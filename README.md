# Telegram Mini App client

A React, TypeScript and Vite client for a Telegram chess Mini App. The game server is not included in this repository.

## Local development

Install Node.js and npm, then install the dependencies:

```sh
npm ci
```

Create `.env.local` with the URL of a compatible Socket.IO server and, optionally, a room ID for local development:

```dotenv
VITE_SERVER_URL=http://localhost:3000
VITE_ROOM_ID=example-room
```

Replace these example values with those for your server and room. The server and its authentication setup are required for gameplay. Vite exposes these variables to the browser, so do not put secrets in them.

Start the client:

```sh
npm run dev
```

Vite listens on port 5173. The client loads Telegram's Web App script and expects the Telegram Web App interface; a browser session alone does not establish a working game.

Other commands:

```sh
npm run build    # TypeScript check and Vite build into build/
npm run lint     # ESLint
npm run preview  # Preview a built client
```

## MagicCraft links

- [Official website](https://magiccraft.io/)
- [Discord community](https://discord.gg/magiccraftgame)
- [Telegram community](https://t.me/magiccraftgamechat)
- [MagicCraft on X](https://x.com/MagicCraftGame)
- [MagicCraft GitHub organization](https://github.com/MagicCraftCompany)
- [Telegram Mini Apps developer documentation](https://core.telegram.org/bots/webapps)
