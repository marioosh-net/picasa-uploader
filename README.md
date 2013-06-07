Picasa Web Albums Console Uploader
==================================

Java console application that upload list of files and/or directories into Google Picasa Web Albums service. It automatically resizes large images to 1600 px or to given value. 

Build
-----

    git clone git://github.com/marioosh-net/picasa-uploader.git
    cd picasa-uploader
    mvn package

Usage
-----

  *List albums*
  
    java -jar picasa-uploader.jar -u <username> -p <password> -l

  *Upload photos to new album*
  
    java -jar picasa-uploader.jar -u <username> -p <password> -t "Spain1" c:\photos\spain1

  *Full syntax*
  
    usage: java -jar picasa-uploader.jar [options] <dir1|file1> <dir2|file2> ...
     -d <description>   album description
     -h                 help
     -l                 list albums
     -p <password>      password [REQUIRED]
     -px <px>           resolution [px], default 1600     
     -t <title>         album title
     -u <username>      user [REQUIRED]
     -v                 be verbose
