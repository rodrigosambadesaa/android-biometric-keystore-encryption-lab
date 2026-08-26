# Biometric + Android Keystore Encryption Lab

Original lab combining `androidx.biometric.BiometricPrompt` with an **auth-per-use Android Keystore AES key**.

- Checks whether strong biometrics can authenticate.
- Creates a non-exportable AES key in `AndroidKeyStore`.
- Encrypts text only after successful biometric authentication through a `CryptoObject`.
- Stores only IV + ciphertext in private `SharedPreferences` for the demo.
- Decrypts via a second biometric-gated cryptographic operation.
- Lets the user delete the key and stored ciphertext.

This is an API demonstration, not a password manager. Real applications must design backup, key invalidation and threat-model-specific storage carefully.
