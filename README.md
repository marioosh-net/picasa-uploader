Picasa Web Albums Console Uploader
===============

1. Build
---

    git clone git://github.com/marioosh-net/picasa-uploader.git
    cd picasa-uploader
    mvn package

2. Usage
---

  *List albums*
  
    java -jar picasa-uploader.jar -u <username> -p <password> -l

  *Upload photos to new album*
  
    java -jar picasa-uploader.jar -u <username> -p <password> -t "Spain1" c:\photos\spain1

  *Full syntax*
  
    usage: java -jar picasa-uploader.jar [options] <dir1|file1> <dir2|file2> ...
     -d <arg>   album description
     -h         help
     -l         list albums
     -p <arg>   password [REQUIRED]
     -t <arg>   album title
     -u <arg>   user [REQUIRED]
     -v         be verbose
