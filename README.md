# Compilation of Tips and Tricks

The intention of this space is to create an easily accessible compendium of useful tips and tricks that I've found throughout the ages while surfing the wonders of the WWW. 







## Command Line Tools

### PDF Compression (macOS & Linux)
Credit: [Max Glenister](https://blog.omgmog.net/post/compressing-pdf-from-your-mac-or-linux-terminal-with-ghostscript/)

Using `ghostscript`, one can compress PDF files through the use of the following command:

```bash
gs -sDEVICE=pdfwrite -dNOPAUSE -dQUIET -dBATCH -dPDFSETTINGS=/screen -dCompatibilityLevel=1.4 -sOutputFile=output.pdf input.pdf
```

### Managing installed libraries
Credit: [crenate](https://stackoverflow.com/questions/8804064/find-opencv-version-installed-on-ubuntu)

Using pkg-config to procure information on installed libraries, e.g., finding out one's OpenCV version:

```bash
pkg-config --modversion opencv
```


## Git Tools

### Update branches
Credit: [John Szakmeister](https://stackoverflow.com/questions/20106712/what-are-the-differences-between-git-remote-prune-git-prune-git-fetch-prune)

Allows one ot update one's local list of remote branches, which I always tend to forget how to do:

```bash
git remote update origin --prune
```


