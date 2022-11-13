# hsif_file_format
The HSIF file format works by saving HEX values in text format. The main extensions are .hsif, .hx and .hxi .
HSIF files are compressed.
The format should be used mostly for vector stuff, but you can use it for bitmaps too.
# Compression
It is best to use compression when you have a basic image. Lines, shapes, etc.
Compression works by:
> Identifying patterns in an image,
> Saving these patterns as commands that will render shapes instead of individual pixels (thus saving on file size),
> Generating a color palette if no more than 30 colors are present in an image, and instead of using the same hex values all the time,
referencing them in the file header as constants.
