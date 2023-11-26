# SteganographyIBM
message hidding in Image
Steganography is the hiding of a secret message within an ordinary message and the extraction of it at its destination. Here we use an image to hide the textual message.

The encoding of the secret content is performed using the well acknowledged encryption algorithm, LSB encoding, which is to perform mainpuation to LSB values of the byte, which in this case is the pixel value R,G and B.

First pixels R value is used to store the lenght of message, the following pixels are used to store the message itself.

JPEG images cannot be used for carrying the message because the hidden content inthe LSB of the image will be lost during compression, thus we must go for some other formats like PNG, where these issue doesnot exist.

The pograms Encoder and Decoder are used to encode and decode secret image into carrier image. Both communicating parties must have the same pair if encoder and decoder program inorder to function properly.

REQUIREMENTS

