# Hextroadinary

Description is the below

> Meet ROXy, a coder obsessed with being exclusively the worlds best hacker. She specializes in short cryptic hard to decipher secret codes. The below hex values for example, she did something with them to generate a secret code, can you figure out what? Your answer should start with 0x.

And these hex values were given to us:

> 0xc4115 0x4cf8

I decided trying to XOR decryption for solve this challange.

Firstly I convert hex values to binary

![HEX TO BINARY](https://github.com/tunahan994/ctf-learn-writeups/blob/main/Writeups/Hextroadinary/img/hex_to_bin_1.png)
![HEX TO BINARY](https://github.com/tunahan994/ctf-learn-writeups/blob/main/Writeups/Hextroadinary/img/hex_to_bin_2.png)

Now I have 2 values. These are

11000100000100010101 for 0xc4115 and 
0100110011111000 for 0x4cf8

For XOR Encryption, values must be has same length. For this reason, I add 0 to the beginning of the shorter value **until their lengths are equal**.
Then I XORed them. (1 for different values and 0 for same values)

```
11000100000100010101
00000100110011111000

11000000110111101101
```

Our new value is 11000000110111101101. Now we must convert this binary value to hex.

![BIN TO HEX](https://github.com/tunahan994/ctf-learn-writeups/blob/main/Writeups/Hextroadinary/img/bin_to_hex_1.png)

Good. Now we have the answer.
Flag is:
**CTFlearn{0xC0DED}**

