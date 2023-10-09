![](assets/images/banner.png)



<img src="assets/images/htb.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Behind Photo</font>

​		DD<sup>th</sup> Month YYYY

​		Challenge Author(s): gospodin69

​		

 



### Description:

On this challenge you need to use beginners tool to decrypt base64 code and after decoding you get md5 hash for all letter individually. After decoding md5 hash you get password for stenographi. Photo.jpeg have secret flag and for decoding Photo.jpeg you need password which is in md5 hash

### Objective

Decode correct for password
### Difficulty:

`very easy`

### Flag:

`HTB{7hank_y0u}`



# Challenge
One day at my cyber security company, an employee downloads a zip file with a photo and unknown text, and we don't know what to do. Can you help us ?



# Solver

```import base64
import sys
import hashlib

with open("password.txt", "rb") as txt:
        decode_string = base64.b64decode(txt.read())
print (decode_string)

##Exported hash decode manualy with online tool

```

