# Personal Diary App

A password-protected, command-line diary that encrypts your entries so only you can read them.

## Features

- Password authentication before accessing your diary
- Entries encrypted with `cryptography` (Fernet symmetric encryption)
- Create, list, and read entries
- A `secret.key` is auto-generated on first run and used to encrypt/decrypt content

## Usage

```bash
pip install cryptography
python app.py
```

Options:

1. **Create a New Entry** - saves an encrypted entry to `entries/`
2. **View All Entries** - lists saved entry files
3. **Read an Entry** - decrypts and displays an entry
4. **Exit** - close the app

## Security Notes

- Change the default password (`Plabon`) in `authenticate()` before using.
- Keep `secret.key` safe - losing it means your entries can no longer be decrypted.
- `secret.key` should never be committed to version control.

## Requirements

- Python 3.x
- `cryptography` package

## License

This project is provided for educational purposes.