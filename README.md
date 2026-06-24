# kpmp-ake-viewer — password-gated viewer

This repository hosts a **single encrypted file** (`index.html`): a password-gated viewer
for a confidential proposal, *Agentic Knowledge Environment for the KPMP Kidney Tissue
Atlas*.

- The dashboard and its PDFs are bundled into one **AES-GCM ciphertext** (PBKDF2 /
  SHA-256 / 200,000 iterations). **Nothing is readable without the password.**
- Decryption happens entirely in your browser. The page is marked `noindex, nofollow`.
- The plaintext proposal lives in a **private** repository; this public repo contains
  only the encrypted blob, which is safe to host openly.

Open the Pages URL, enter the password (shared separately), and the full interactive
dashboard renders locally in your browser.
