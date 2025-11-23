# Contributing to QWallet

Thanks for wanting to contribute! This document describes how to get the project running locally, how to submit code, and our expectations.

1. Code of conduct
- Be respectful, constructive, and inclusive.

2. Getting started
- Install Rust:
  - curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  - rustup default stable
  - rustup update
- Install Node.js (LTS) using nvm or the installer: https://nodejs.org/
- Install Tauri CLI (one of):
  - cargo install tauri-cli
  - npm install -g @tauri-apps/cli

3. Local development
- If there's a frontend directory:
  - cd frontend
  - npm ci
  - npm run dev (or the project-specific start)
- From project root:
  - cargo tauri dev
  - cargo test
  - cargo tauri build

4. Branching and pull requests
- Use branch names like `feature/<short>` or `fix/<short>`.
- Open a PR with a clear description, tests, and screenshots where applicable.
- Add `Closes #<issue-number>` when the PR fixes an issue.

5. Tests and CI
- Run Rust tests: `cargo test`
- Run frontend tests (if any): `npm test` in the frontend directory
- Add unit and integration tests for new behavior.

6. Commits
- Keep commit messages short and descriptive.
- Include a more detailed message body when needed.

7. Security and secrets
- Never commit private keys, secrets, or credentials.
- If you discover a security issue, follow SECURITY.md.

Thank you for contributing!
