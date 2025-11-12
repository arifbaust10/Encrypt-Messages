# Encrypt-Messages

**An Efficient Implementation of Classical and Modern Encryption Methods for SMS Messages**

---

## **Project Overview**
This project demonstrates the implementation and comparison of **six encryption algorithms** on a dataset of SMS messages. The goal is to secure messages by transforming them into encrypted ciphertexts and storing corresponding keys for each method.

**Encryption Methods Included:**
1. **Vigenere Cipher** – Classical polyalphabetic substitution cipher.
2. **Vernam Cipher** – Bitwise XOR with a repeating key.
3. **One-Time Pad (OTP)** – XOR with a random key of the same length as the message (perfect secrecy).
4. **DES (Data Encryption Standard)** – Symmetric block cipher using 64-bit blocks.
5. **AES (Advanced Encryption Standard)** – Symmetric block cipher (128-bit key, CBC mode with IV).
6. **RSA Hybrid Encryption** – AES encrypts message; AES key is encrypted with RSA public key.

---

## **Dataset**
- **Source:** SMS messages collected manually (both spam and ham).  
- **Columns:**
  - `Label` – Indicates whether the message is spam or ham.
  - `Message` – Full text of the SMS.  
- **Format:** CSV file (`new.csv`) with headers `Label` and `Message`.

**Note:** Data was collected using **AirDroid** to extract messages from a mobile device.

---

## **Workflow**
1. Read the CSV dataset using Python (`pandas`).  
2. Preprocess messages (convert to strings, handle missing values).  
3. Encrypt each message using six different algorithms.  
4. Save ciphertexts and corresponding keys into a new CSV (`new_encrypted.csv`).  
5. Review results for correctness and reproducibility.

**High-Level Workflow Diagram:**

<img width="875" height="293" alt="Screenshot 2025-11-12 at 7 30 05 PM" src="https://github.com/user-attachments/assets/0124647b-fbd3-491b-806d-3d6dc4f844da" />


