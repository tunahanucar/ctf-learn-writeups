# Snowboard

We have a description and a photo (Snowboard.jpg)

I don't see anything on photo. Let's look at metadata (using exiftool).

![EXIFTOOL](https://github.com/tunahan994/ctf-learn-writeups/blob/main/Writeups/Snowboard/img/exif.png)

Hmm that was a little weird. I knew it was easy but not this much.

Yes, just as I expected. This flag is wrong. Let's keep searching.

After the metadata, I thought of looking at their strings.

![STRINGS](https://github.com/tunahan994/ctf-learn-writeups/blob/main/Writeups/Snowboard/img/base64.png)

Is it a base64 code? Looks a bit suspicious. Let's decode it

![BASE64](https://github.com/tunahan994/ctf-learn-writeups/blob/main/Writeups/Snowboard/img/decoded.png)

Yeah flag must be this.

Flag is:
**CTFlearn{SkiBanff}**
