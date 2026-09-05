[![Termphin - an SSH client whose sessions survive the dropped connection](https://termphin.dev/gh-banner.webp)](https://termphin.dev)

# Termphin

Termphin is an SSH client. It connects your device to your servers, lets you run
commands, browse and edit files, and keeps sessions alive when you switch apps
or lose signal.

**This repository is the issue tracker.** The app's source is not here - it is
where you report a bug, ask for a feature, or ask a question.

- [Report a bug](../../issues/new?template=bug_report.yml)
- [Suggest an idea](../../issues/new?template=idea.yml)
- [Manual](https://book.termphin.dev) · [Website](https://termphin.dev) · [Changelog](https://termphin.dev/changelog)

## What it does

- A terminal that renders text interfaces correctly, including diffs, progress bars and spinners.
- Fourteen colour schemes, light and dark, with adjustable font size, line height and padding.
- An SFTP browser in the same tab as the shell: walk the filesystem, edit files with syntax highlighting, preview images and upload from your device.
- Port forwarding - local and remote tunnels, opened per session or saved with a profile.
- Snippets: save commands you use often and run them with one tap on any machine.
- An SSH key manager: generate ed25519 and RSA keys or import your own, kept encrypted on the device behind a PIN or fingerprint.
- Jump hosts, the way OpenSSH's ProxyJump works - point a profile at another profile.
- A draggable action dock you lay out yourself.

A small agent on the server keeps your shell running through a dropped
connection or a switched network, and Termphin reattaches you to the same
session when you come back. A server reboot still ends that shell; you land in
a fresh one in the same directory.

Keys and profiles never leave the device. The only thing Termphin sends anywhere
is anonymous usage analytics, and only if you say yes when asked.

## Before you open an issue

- Check the [manual](https://book.termphin.dev) - it covers connections, keys, files, tunnels and the remote agent.
- Search the existing issues; a comment on the open one is more useful than a second report.
- Never paste a private key, a password or a real host key. Redact hostnames and usernames if you would rather not share them - the app's **Anonymize** switch in Settings does this for screenshots.

## Other Termphin repositories

- [terminal_view](https://github.com/Termphin/terminal_view) - the terminal widget the app renders with
- [termphin-agent](https://github.com/Termphin/termphin-agent) - the server-side agent that keeps sessions alive

## Security

Do not open an issue for a vulnerability. See [SECURITY.md](SECURITY.md).
