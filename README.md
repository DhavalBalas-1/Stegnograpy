# README: Image-Based Steganography

## Overview
This Python script performs basic steganography by embedding a secret message into an image and later retrieving it using a passcode. It modifies pixel values to store the message and requires the correct passcode to decrypt it.

## Prerequisites
Ensure you have the following dependencies installed:

- Python 3.x
- OpenCV (`cv2`)
- OS module (included in Python standard library)

To install OpenCV, use:
```sh
pip install opencv-python
```

## How It Works
1. The script reads an image (`test sample.jpg`).
2. It takes user input for a secret message and a passcode.
3. The message is encoded into the image by modifying pixel values.
4. The modified image is saved as `encryptedImage.jpg`.
5. The script then prompts for the passcode to decrypt the message.
6. If the passcode is correct, the original message is extracted and displayed.

## Usage
### Encrypt a Message:
1. Place `test sample.jpg` in the script directory.
2. Run the script:
   ```sh
   python script.py
   ```
3. Enter the secret message when prompted.
4. Enter a passcode to secure the message.
5. The script saves an encrypted image as `encryptedImage.jpg`.

### Decrypt a Message:
1. Run the script again.
2. Enter the passcode when prompted.
3. If correct, the original message is displayed.

## Notes
- Ensure `test sample.jpg` exists in the working directory.
- Only text characters within the ASCII range (0-255) are supported.
- The encryption method is not secure for high-level cryptographic purposes.

## Disclaimer
This script is for educational purposes only. Do not use it for storing sensitive or confidential data.

