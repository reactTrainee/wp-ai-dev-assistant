# WP AI Dev Assistant

An open-source, early-stage AI developer assistant for WordPress.

## What it does

The MVP adds a WordPress admin tool for:

- WordPress/PHP error analysis
- Debugging guidance
- Code explanation
- WordPress hook/filter generation
- General WordPress development questions

The initial AI provider integration uses the Anthropic Claude API.

## Project goal

Reduce the time WordPress developers spend diagnosing errors and searching across documentation, issue trackers, logs, and code examples.

## Repository layout

- `wordpress-plugin/` — installable WordPress plugin
- `docs/` — product and technical documentation
- `website/` — initial landing page

## MVP setup

1. Install the plugin from `wordpress-plugin/wp-ai-dev-assistant/`.
2. Activate it in WordPress.
3. Go to **WP AI Dev Assistant → Settings**.
4. Add a Claude API key.
5. Select a supported Claude model.
6. Open **WP AI Dev Assistant** and test an error or development question.

## Development principles

- Keep API credentials server-side.
- Use WordPress nonces and capability checks.
- Avoid destructive troubleshooting recommendations.
- Do not send sensitive credentials or private customer information to an AI provider.
- Keep the AI provider integration replaceable where practical.

## Roadmap

- [x] Initial plugin architecture
- [x] Server-side Claude API request
- [x] Admin troubleshooting UI
- [x] Settings page
- [ ] Debug log upload/analysis
- [ ] Conversation history
- [ ] Prompt templates
- [ ] Better Markdown rendering
- [ ] Provider abstraction
- [ ] WordPress.org packaging improvements
- [ ] Public beta

## Status

Early-stage MVP. Not yet recommended for production environments without additional security, privacy, testing, rate limiting, logging controls, and secret-management review.

## License

MIT for project-level materials. The WordPress plugin is GPL-2.0-or-later to align with WordPress plugin distribution requirements.
