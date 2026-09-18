# Steam Account Import Formatter

A browser-based tool for converting bulk Steam account data into an import-ready format.

## Features

- Parse multiple account records at once
- Accept labeled source text and `--` / `---` / `----` delimited rows
- Accept four-field rows without a game ID
- Convert escaped email addresses such as `name\@example.com`
- Generate one import-ready account per line
- Optionally use the Steam username as the game ID
- Process all data locally in the browser

## Usage

Open `dist/index.html` in a modern browser, paste the source account data, and copy the formatted result into the account launcher's bulk input field.

The generated format is:

```text
username---password---email---email_password---game_id
```

## Deployment

This is a static site. Serve the `dist` directory with any static web server.
