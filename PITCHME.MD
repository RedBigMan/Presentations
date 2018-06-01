#Cryptopals

---
### Set 1
 ---
### Challenge 1

- Converts Hex to Base64
---
### Challenge 2

- Introduction to XOR operation.
- Types become important
---

### Challenge 3
- XOR'd cipher
- Knowing that it was a message,
- I printed the one that contained at least 5 spaces
---
### Challenge 4
- Same principles as 3.
- needed extra filters to remove plaintext containing special characters.
---
### Challenge 5
- Similar to 3 & 4, challenge 5 introduced a keysize > 1.
- To accomplish this, converted each char to byte then XOR'd.
---
### Challenge 6
- This challenge is where the difficulty picked up.
- To find the plaintext, I needed to find the keysize then check each character.
- keysize was found using a hamming function.
- Scoring each character based on letter frequency, I picked the ones with the highest score.
- After finding the key, I used the key to decipher the entire file at a faster rate.
---
### Challenge 7
- Introduction to ECB.
- This challenge was to simply decrypt an AES-128 cipher in ECB mode.
- Used built-in python library to achieve this.
---
### Challenge 8
- Detecting ECB mode
- This detection was simple, apply the same principles that let you see a penguin.
- I compared each block to look for ones that are identical
- While still possible with other encryption techniques, it is very improbable.
---
### Set 2
---
### Challenge 9
- Challenge was to implement PKCS#7 padding.
- Achieved by appending the hex value of n, n times.
---
### Challenge 10
- Challenge was to implement AES-128 CBC encryption.
- Used python modules to achieve this.
---
###Challenge 11
- Needed to create a detection oracle for CBC and ECB.
- Knowing that it is either one or the other, I checked for ECB and printed the identical lines.
- If after the check there was no identical lines, I can conclude the cipher is CBC
---
### Challenge 12
- Byte at a time ECB
- To achieve this challenge, I first needed blocksize.
- After, I iterated through blocksize-n to find the plaintext of each block independently.
---
###Challenge 13
- This challenge was to change contents of a string from user to admin.
- Given the information, key, and the function profile_for()
---
###Challenge 14
- Challenge 12 but harder
- needed to find blocksize by looking for when encrypted_file size jumped.
- because prefix is static after startup, once prefix is found, same operation as 12
---
###Challenge 15
- Checks for padding and removes if valid.
- If not valid returns error.
---
###Challenge 16
- Bit-flipping attack
- requires editing of previous value so that the XOR operation produces wanted results.
---
