This is the Adventure Builder Colouring Book taken from the [original JPG files](https://www.dropbox.com/s/d76ig7ep6xep7rz/ColouringBook.zip?dl=0) and converted to a browsable [GitBook](https://www.gitbook.com).

Conversion was done by:

```
for fn in `find . ! -path .`; do echo "Converting $fn to SVG"; convert -channel RGB -compress None $fn bmp:- | potrace -s - -o $(basename $fn .jpg).svg; done
```
