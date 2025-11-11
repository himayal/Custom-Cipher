# Custum-Cipher

Custom Cipher – Affine + Rail-Fence
This project implements a two-stage classical encryption system combining the Affine Cipher and the Rail-Fence Cipher, along with basic cryptanalysis (known-plaintext attack).

Project Files               File	Description
Custom_Cipher.ipynb	        Encryption and decryption of text using Affine + Rail-Fence
Demo_Custom_Cipher.ipynb	  Interactive demo for encrypt/decrypt
Attack_Custom_Cipher.ipynb  Performs known-plaintext attack on the cipher

How It Works:
Encryption Process
Step 1 → Affine Cipher: converts each letter using formula E(x) = (a*x + b) mod 26
Step 2 → Rail-Fence Cipher: rearranges letters in a zigzag pattern across rails

Decryption Process:
Step 1 → Reverse Rail-Fence pattern
Step 2 → Reverse Affine formula D(x) = a⁻¹ * (x − b) mod 26

Attack:
Performs known-plaintext attack to guess keys by comparing a known portion of plaintext with ciphertext.
