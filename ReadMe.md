
**# PDF Password Manager (Desktop UI)**

A tiny Windows desktop app (Tkinter) that manages PDF passwords - both remove and add password protection. Your original files are never modified.

Use this responsibly and only on PDFs you own or have permission to modify.

## ✨ Features
**Remove Password Protection:**
- Select a password‑protected PDF
- Enter the existing password
- Choose where to save the unlocked copy

**Add Password Protection:**
- Select an unprotected PDF
- Set a new password with confirmation
- Choose where to save the protected copy

**Additional Features:**
- Tabbed interface for easy switching between operations
- Close button and status prompts
- Pleasant light theme with optional logo (PNG/ICO)
- Clickable support link: `www.analysis.ie/contact`

## 🚀 How to use the app

**Remove Password Tab:**
1. Click "Browse…" to pick the password-protected PDF
2. Enter the existing password
3. Click "Browse…" to choose the output file (defaults to `_unlocked.pdf`)
4. Click "Remove Password"
5. Success message shows the saved path

**Add Password Tab:**
1. Click "Browse…" to pick an unprotected PDF to protect
2. Enter your new password
3. Confirm the new password
4. Click "Browse…" to choose the output file (defaults to `_protected.pdf`)
5. Click "Add Password"
6. Success message shows the saved path

**Notes:**
- If the PDF isn't encrypted during removal, a plain copy is created
- Incorrect passwords show clear error messages
- Password confirmation prevents typos when adding protection
- Large PDFs may take time to process

## 🔒 Security & privacy
- All processing happens locally on your machine. No data is uploaded.
- Only use this on documents you own or are authorized to modify.
- Passwords are handled securely in memory and never stored or logged.

## 🧰 Dependencies
- [PyPDF2](https://pypi.org/project/PyPDF2/) — reading/writing PDFs
- [PyCryptodome](https://pypi.org/project/pycryptodome/) — AES used by some PDFs
- Tkinter — included with standard Python on Windows

## 🧩 Troubleshooting
- “PyCryptodome is required for AES algorithm” → ensure `pycryptodome` is installed
- SmartScreen blocks the EXE → “More info” > “Run anyway”, or code‑sign the EXE
- Save errors → verify you have write permissions and the target file isn’t open elsewhere
- Logo not showing in EXE → include `assets/logo.png` before building or place `logo.png` next to the EXE

## 📫 Support
Questions or feedback: https://www.analysis.ie/contact
