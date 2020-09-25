# key-extraction-from-images

Implementation:
Extracting String from image
Input: Image of any size.
Procedure: convert the rgb image to gray image and set the threshold. Resize the image to required dimension and store the binary values of the image based on the threshold.

Extract the key from HMAC sha256 generator and store in a file.

Extract the key from string and HMAC key.
#test case 1
secret_key = secretkey_generate(“0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b0b","Hi There")
length of key 20
length of message 8
secret key generated : b0344c61d8db38535ca8afceaf0bf12b881dc200c9833da726e9376c2e32cff7
#test case 2
secret_key = secretkey_generate("4a656665","what do you want for nothing?")
length of key 4
length of message 28
secret key generated  : 5bdcc146bf60754e6a042426089575c75a003f089d2739839dec58b964ec3843
Reference Websites for validating test cases
https://www.liavaag.org/English/SHA-Generator/HMAC/
https://cryptii.com/pipes/hmac
Test case proving the outcomes in RFC are correct:
https://stackoverflow.com/questions/16232040/testing-hmacsha256-signature
