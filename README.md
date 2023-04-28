<h1 align="center">
  <br>
  <span> :male_detective: CoVerT :female_detective: </span>
  <br>
  
  [![](https://img.shields.io/badge/Made_with-Python3-blue?style=for-the-badge&logo=python)](https://www.python.org "Python3")[![](https://img.shields.io/badge/Made_with-Flask-blue?style=for-the-badge&logo=Flask)](https://flask.palletsprojects.com/en/1.1.x/ "Flask")

</h1>
<span><h4 align="center">The Cloak of Invisibility for your texts</h4></span>

<p align="justify">
CoVerT is a steganography technique implemented in python, to hide secrets inside text by encrypting the secret before cloaking it with special unicode invisible characters. 
It can be used to safely watermark strings, invisible scripts on webpages, texts on social media or for any other covert communication. Completely invisible! 
<p>

## Resources 

The following paper was implemented for generating and embedding Zero Width Characters in cover message and extracting the secret message from the cover message and generating ascii from extracted Zero Width Characters. 



- Taleby Ahvanooey, Milad & Li, Qianmu & Hou, Jun & Dana Mazraeh, Hassan & Zhang, Jing.
```
AITSteg: An Innovative Text Steganography Technique for Hidden Transmission of Text Message via Social Media.
IEEE Access
```

## Features
- Protect your invisible secret using passwords
- Cryptographically secure by encrypting the invisible secret using AES-256-CTR encryption and decryption.
- Uses Invisible characters in unicode characters that works everywhere in the web - Tweets, Gmail, WhatsApp, Telegram, Instagram, Facebook, and many more!
- Completely invisible, uses Zero Width Characters instead of white spaces or tabs.
- The secret message which is encrpted using password can be embedded in the cover message by the sender and extracted from the cover message and decrypted using the same password by the receiver.

<br>

## Functions implemented
- Embed algorithm: To embed the secret message into the cover message by converting it into invisible zero width unicode characters.
- Extract algorithm: To extract the secret message from the cover message by converting it back into ascii characters from invisible zero width unicode characters.
- AES-encryption: We take password for encrypting the secret message before embeding it,the key for encryption is generated from the password based key derivation function PBKDF2.
- AES-decryption: For decrpytion,we need to pass the same password used while encryption since AES-256 is a symmetric cipher.

#### Installation
Install the dependency for AES by running:
```html  
    pip install pycryptodomex
```

#### Run using Command Prompt
Clone the repository and run the following commands-
```html
    set FLASK_ENV=development
    set FLASK_APP=app.py
    flask run
```
## Steganography is not Cryptography ! :confused:

If you are getting confused between _Steganography_ & _Cryptography_. Then see this -

#### Cryptography

**If** `you = wms` **then** `Qcaapgrw gq gknmprylr` **= ?**<br>
_Can you guess the answer?_<br>
Here we have `key = -2` i.e. if we go 2 alphabets behind `y` you get
`w` and similarly if you go 2 alphabets behind `o` we get `m` and similarly 2 alphabets behind `u` gives us `s`. Therefore `you = wms`. <br>
So now you may have got the answer which is `Security is important`.
> Note: The cryptography algorithms are much advanced now.

#### Steganography

So now that you know what is cryptography so lets know what is _Steganography_.<br>
**If** `____=____` **then** `______=______` **?**<br>
_Confused ?_<br>
Here you won't be able to even sense the presence of data. Leave alone knowing what
is the data. That's why it is called hiding data in plain sight. There are some applications which
may detect the presence of hidden data. CIA obviously has it <emoji><br>
Generally at professional level the data hidden is encrypted first. So _steganography_ and _cryptography_ are not
mutually exclusive to each other.
>Knowledge fact: Jeff Bezos's mobile was hacked by hiding malicious code in a media
>file which on getting downloaded sent the host device's control to the hacker.

###             Tech stack
`Backend` : Python3,Flask  <br>
`Frontend` : Html,CSS  <br>

<h3 align="center"><b>Developed with :heart: by <a href="https://github.com/debjit20504">Debjit Pramanik</a></b>, <b><a href="https://github.com/sahil20115">Sahil Kumar</a></b>


