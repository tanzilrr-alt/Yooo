# Personal AI — iPhone PWA

A no-Mac starter that runs directly in Safari and can be added to the iPhone Home Screen.

## Included
- Password unlock; no Face ID
- AES-256-GCM authenticated encryption
- Random 256-bit cryptographic key derived from the password
- Random 128-bit salt and unique IV per encryption
- PBKDF2-SHA-256 with 600,000 iterations
- IndexedDB local storage
- Local-only chat UI
- No hard-coded encryption key
- No network calls in the included app code

## Important security limitation
This is a browser/PWA security design, not the same security boundary as a native iOS app using Keychain/Secure Enclave. Safari storage and JavaScript are subject to the browser's security model. Do not treat this starter as certified, military-grade, or unbreakable.

## Install on iPhone
1. Put this folder on any HTTPS web host.
2. Open the HTTPS URL in Safari on iPhone.
3. Tap Share -> Add to Home Screen.
4. Create a strong 14+ character password.
5. Do not lose the password: there is no recovery mechanism.

For private testing, use a trusted HTTPS host. Do not host this app on an untrusted site.
