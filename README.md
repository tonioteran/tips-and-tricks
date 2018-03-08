# Compilation of Tips and Tricks

The intention of this space is to create an easily accessible compendium of useful tips and tricks that I've found throughout the ages while surfing the wonders of the WWW. 







## Command Line Tools

### Reformatting Images



### Resizing Images
Credit: [Rinzwind](https://askubuntu.com/questions/271776/how-to-resize-an-image-through-the-terminal)

To quickly resize an image using ```convert```, it's as simple as:

```bash
convert figure.png -resize 128x128 resizedFigure.png
``` 

### Convert Image Set Into Video
Credit: [Hammad Mazhar](http://hamelot.io/visualization/using-ffmpeg-to-convert-a-set-of-images-into-a-video/)

The previous list contains a pretty comprehensive list for accomplishing this by using `ffmpeg`.

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


## IPython

### Apply changes after edits
Credit: [Andrew](https://stackoverflow.com/questions/1254370/reimport-a-module-in-python-while-interactive)

I was always very annoyed whenever changes to my files wouldn't be recognized during an ipython session (so much time spent debugging thinking there was an error in my code, when the only issue was that the changes weren't being taken into account). Using the [autoreload](https://ipython.readthedocs.io/en/stable/config/extensions/autoreload.html) extension, one is able to have the modules automatically reloaded before executing user code.

```python
%load_ext autoreload
%autoreload 2
```

