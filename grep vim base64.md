# Crptography Regex and vim

### **Crytography**

There are many cryptography tools and algorithms out there but for now lest focus on `base64` since it is built in to the cli. but there are many such as.
**Encoding**

* Base64, 32, and 16
* URL Encoding
* Hex to ASCII to OCTAL interchange

**Ciphers**

* Morse
* Letter Numbers
* Caesarian Shift
* ROT13
* Baconian
* Vigenere
* Hill

For `base64`, encoding and decoding them comes easy in kali linux terminal/cli.
heres and example.

```
echo  'hello world' | base64
```

On this example we printed out the result of 'hello world' to a base64 format.
Subsequently we can also decode a base64 string back ASCII. For example.

```
echo "aGVsbG8gd29ybGQK" | base64 -d
```

in this case we added the `-d`option.
You can also do this for base32

```
echo  'hello world' | base32
echo 'JBSWY3DPEBLW64TMMQFA====' | base32 -d
```

for more encrypting and decrypting tools we can use **cyberchef** software.
**more info can be found here [https://charcharbinks.com/post/ctf\_crypto\_for\_beginners/](https://charcharbinks.com/post/ctf_crypto_for_beginners/)**

### **RegEx**

this one is quite fun. you'll see why.
Regex is used to carve out data from a dump. this helps you to isolate information that are only neccessary to your needs.
**for this one, theres a very good training website here : [https://regexone.com](https://regexone.com)**
**Master The art of Regex and become a infoGod. Take as how many tries as you want.**

### **VIM**

Ah yes, `vim`. the infamous text-based editor. CTF's this is not realy necessary. of course you can use nano and mousepad as your text editor. But, Master `vim`. You become a keyboard Warrior Free from the binds of mouse.
Perks?

* Insane Cursor Movement Speed
* Can Portal to Specific Sections of a text dump
* Supper lightweight software

There are now modern versions of `vim`, and that is neovim or `nvim` for short.
type the command `vim` or `nvim` in your terminal then youl be greeted with `vim`
Keeping tradition I won't Tell you how to exit `vim`.
**For practicing vim in a safe space go to this website: [https://www.openvim.com](https://www.openvim.com)**
Have some fun at it.

#### UP NEXT: KALI-LINUX DIGITAL FORENSICS TOOLS, PW CRACKING SOFTWARES AND WORDLISTS.