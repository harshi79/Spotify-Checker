# 🎵 Cookie Checker

A multi-threaded cookie validation utility with proxy rotation, retries, account-detail extraction, and optional Discord or Telegram notifications.

## Features

- Fast multi-threaded cookie checking
- Netscape `.txt` and JSON cookie input support
- Account plan, email, country, account-role, and payment-detail extraction
- Broad HTTP and SOCKS proxy format support
- Retry handling with proxy rotation
- Built-in email deduplication
- Log and dashboard display modes
- Optional Discord and Telegram notifications
- Organized outputs by run, plan, and account role

## Requirements

```bash
pip install -r requirements.txt
```

Optional SOCKS support:

```bash
pip install 'requests[socks]'
```

## Quick start

1. Clone this repository.
2. Install dependencies with `pip install -r requirements.txt`.
3. Place authorized cookie files in `cookies/`.
4. Optionally add proxies to `proxy.txt`.
5. Configure `config.yml`.
6. Run `python main.py`.

## Folder layout

```text
cookies/         # input cookies
failed/          # invalid or expired inputs
broken/          # malformed or error cases
hits/            # successful outputs
proxy.txt
config.yml
main.py
```

## Configuration

`config.yml` controls output fields, notification settings, display mode, and retry attempts. Webhook and Telegram notifications are disabled by default.

## License

MIT License. See `LICENSE`.

## Disclaimer

Use this tool only with accounts and cookie files you are explicitly authorized to test.
