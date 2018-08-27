# dl2dir
A personal script to Download Weblinks with axel to subfolders in a base directory. Configured for mp4, but can be used for any file.

This will be enhanced with optional download methods.
Primary use is intended for downloading media files that I can seperated into subfolders.
example for mp4:
dl2dir -B "${HOME}/Videos" -D "Movies/The Lion King (1994)" -T "The Lion King (1994 - WEBDL" -L "http:/link.com/to/file.mp4"
  This will download "http:/link.com/to/file.mp4" to "$HOME/Videos/Movies/The Lion King (1994)/The Lion King (1994) - WEBDL.mp4"
Example for pdf:
dl2dir -B "${HOME}/Documents" -D "PDF" -T "mydownload.pdf" -e pdf -L "http:/link.com/to/file.pdf"
  this will download "http:/link.com/to/file.pdf" to "$HOME/Documents/PDF/mydownload.pdf"
  
  
  IF the File already exist, the file will be renamed with an appended date and time stamp such as
    file.mp4 > file.180826144559.mp4
