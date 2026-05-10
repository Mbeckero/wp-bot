# wp-bot

A WhatsApp bot for automating messages, responses, and workflows.

## Overview

`wp-bot` is a WhatsApp automation bot built to handle incoming messages, send automated replies, and integrate with external services. It leverages the WhatsApp Web API to interact with chats programmatically.

## Features

- Automated message responses with custom rules
- Command-based interactions (e.g. `/help`, `/status`)
- Group and private chat support
- Webhook integration with external services
- Configurable via environment variables

## Requirements

- Node.js >= 18
- A WhatsApp account (personal or Business)
- A phone with WhatsApp installed (for QR-code session authentication)

## Installation

```bash
git clone https://github.com/mbeckero/wp-bot.git
cd wp-bot
npm install
```

## Configuration

Copy the example environment file and fill in your values:

```bash
cp .env.example .env
```

| Variable          | Description                                         |
|-------------------|-----------------------------------------------------|
| `SESSION_NAME`    | Name for the WhatsApp session                       |
| `WEBHOOK_URL`     | URL to forward incoming messages (optional)         |
| `PREFIX`          | Command prefix character (default: `/`)             |
| `OWNER_NUMBER`    | Bot owner's phone number (e.g. `5491112345678`)     |

## Usage

Start the bot and scan the QR code with your phone:

```bash
npm start
```

On first run a QR code will appear in the terminal. Open WhatsApp > Linked Devices > Link a Device and scan it.

## Development

```bash
npm run dev
```

Run tests:

```bash
npm test
```

## Project Structure

```
wp-bot/
├── src/
│   ├── commands/   # Individual command handlers
│   ├── handlers/   # Event and message handlers
│   └── index.js    # Entry point
├── .env.example
└── package.json
```

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "add my feature"`
4. Push and open a pull request

## License

MIT
