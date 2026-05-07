# wp-bot

A bot for automating WordPress tasks and interactions.

## Overview

`wp-bot` is a tool designed to automate common WordPress operations, such as content management, publishing workflows, and site maintenance tasks.

## Features

- Automated post/page creation and publishing
- Content scheduling and management
- WordPress REST API integration
- Configurable via environment variables

## Requirements

- Node.js >= 18 (or Python >= 3.10, depending on the stack)
- A WordPress site with REST API enabled
- Application Passwords or JWT authentication configured on WordPress

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

| Variable              | Description                                  |
|-----------------------|----------------------------------------------|
| `WP_URL`              | Base URL of your WordPress site              |
| `WP_USER`             | WordPress username                           |
| `WP_APP_PASSWORD`     | WordPress Application Password              |

## Usage

```bash
npm start
```

## Development

```bash
npm run dev
```

Run tests:

```bash
npm test
```

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "add my feature"`
4. Push and open a pull request

## License

MIT
