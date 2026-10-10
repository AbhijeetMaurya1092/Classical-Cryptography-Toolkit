# Midnight Cipher
A self-contained HTML/CSS/vanilla JavaScript classical cryptography laboratory. Open index.html directly in a modern browser; no installation or server is needed. Keep index.html, style.css, script.js and README.md together.

Eight actual encrypt/decrypt implementations: Caesar, Monoalphabetic, Playfair, Hill (2×2), Vigenère, One-Time Pad, Rail Fence and Columnar Transposition. Three switchable neon interfaces, CSS 3D reactor, operation scan animation and optional browser-synthesized sound. File import, output copy/download, swap, reset, current-data visualizations, measured benchmarks and local metadata history are included.

Key formats and algorithm-specific text handling are documented in the in-app field guide and beside each key input. Playfair normalizes letters, merges J/I, and inserts X or Q fillers. Hill normalizes letters and pads odd messages with X. Neither can reconstruct discarded formatting or remove fillers unambiguously. Transposition operates on all Unicode characters without padding. Caesar, substitution, Vigenère and OTP preserve non-English-letter characters.

Choose a method, input text, provide the key and choose Encrypt or Decrypt. Import .txt files locally via File processing; download the workspace output after processing. Clipboard access may depend on browser permissions; a fallback is attempted. Audio requires an explicit Sound on click. Reduced-motion preferences disable decorative motion. Recent metadata history is limited to 50 operations; dashboard counts reflect retained history. No keys or plaintext are stored in history; clear history removes those local records.

Click Run self-tests in the Field guide for known vectors, round trips, padding, duplicate column keywords and invalid-key rejection. Benchmarks run 100 encryptions per method on the current input using educational sample keys, and report average compute time. They do not measure security.

Classical ciphers are educational and unsuitable for modern confidential communication. True OTP security requires a uniformly random secret key never reused. All provided samples are educational.

Validation: JavaScript syntax and automated algorithm checks run with Node as a development test tool; Node is not an application dependency. Browser UI, audio, clipboard and responsive visual QA were not executed in this environment.

## Cyrix companion
The animated CSS cyber-bot greets visitors on landing, follows mouse movement, reacts to processing and errors, and offers a local chat panel with built-in help for the supported toolkit topics. It is a rule-based assistant, not a connected language model. Error suggestions require an explicit Apply button and never silently replace a key. OTP key generation uses crypto.getRandomValues with rejection sampling for unbiased A–Z letters. Decryption still requires the original encryption key; the bot cannot recover unknown keys. Chat stays in memory, has no network requests, and is not persisted.


## Live demo
[Open Midnight Cipher](https://midnight-cipher-abhi-neon.bloomy-rain-8456.chatgpt.site)
