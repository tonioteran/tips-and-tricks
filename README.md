# Compilation of Tips and Tricks

The intention of this space is to create an easily accessible compendium of useful tips and tricks that I've found throughout the ages while surfing the wonders of the WWW. 



## Command Line Tools

### PDF Compression (macOS & Linux)
Credit: [Max Glenister](https://blog.omgmog.net/post/compressing-pdf-from-your-mac-or-linux-terminal-with-ghostscript/)

Using `ghostscript`, one can compress PDF files through the use of the following command:

```bash
gs -sDEVICE=pdfwrite -dNOPAUSE -dQUIET -dBATCH -dPDFSETTINGS=/screen -dCompatibilityLevel=1.4 -sOutputFile=output.pdf input.pdf
```


