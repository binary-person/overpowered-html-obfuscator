# Overpowered HTML obfuscator
Turn your 21 bytes file into a 73.72MB file!

Why did I ever do this? Don't ask....

The usage is as follows:
```
node index.js input_file output_file number_of_wraps number_of_recursive_wraps
```

### number\_of\_wraps
This option simply determines the amount of times base64(encodeURIComponent(base64(code))) should be wrapped.

### number\_of\_recursive\_wraps
Highly not recommended to set this value at a high number since a max call stack error may occur. This is where the size of the output file really starts to skyrock.

### Few notes
You can turn those values as high as you want, until the memory or the hard drive runs out of space.<br>
A few use cases might be: making sure that no one views your source code (I mean, technically, since they could also just *try* to open up chrome dev tools), obfuscating, or simply inflating your file.


Have fun!<br>
Simon Cheng