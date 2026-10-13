# SafeKey

SafeKey is a small, browser-based password generator. Select **Generate password** to create a new 16-character password containing uppercase letters, lowercase letters, and numbers. Select the copy button to copy the generated password to your clipboard.

## Privacy and security

- Passwords are generated in your browser with the Web Crypto API (`crypto.getRandomValues`); they are not sent to a server.
- Random bytes are sampled without modulo bias so each character in the alphanumeric alphabet is equally likely.
- The page does not save or transmit generated passwords.
- Clipboard access depends on browser support and security settings. If copying is unavailable, the password remains visible so it can be copied manually.

## Run

Open `index.html` in a modern browser. Clipboard support may require a secure context, such as HTTPS or localhost.

## Contents

- `index.html` — the complete responsive interface, styles, and password-generator logic.
