# cmus-lyrics
**cmus-lyrics** is a simple bash script that fetches the lyrics of current song playing in [CMus] (C* Music Player).

This version is based on https://github.com/hakerdefo/cmus-lyrics

The most important changes are
 - code clean-up
 - add caching
 - add better lyrics formatting

### Dependencies :
- Perl - Perl (Practical Extraction and Reporting Language) originally developed by Larry Wall is a family of high-level, general-purpose, interpreted, dynamic programming languages. [Perl] is available in repositories of almost every Linux distribution under the sun. Use your distribution's package manager to install it. Perl Module [URI::Escape] is needed.
- Wget - [Wget] is a free software package for retrieving files using HTTP, HTTPS and FTP, the most widely-used Internet
protocols. Most Linux distributions have Wget in their package repositories so you can easily install Wget via the package manager of your distribution in case it is not installed on your system.
- Some more-or-less common Linux tools (grep, sed, vim), which are detected automatically.

### Installation :
Download [cmus-lyrics-master.zip],

```sh
wget https://github.com/aswna/cmus-lyrics/archive/master.zip
```

Extract it,

```sh
unzip cmus-lyrics-master.zip
```

Create a **${HOME}/bin** directory, if it does not exist already.
Add this directory to your **${PATH}**.
Make **cmus-lyrics** executable and copy it to **${USER}/bin** directory,

 ```sh
mkdir -p ${HOME}/bin
export PATH=${PATH}:${HOME}/bin  # put this to one of your .rc files
cp cmus-lyrics-master/cmus-lyrics ${HOME}/bin/
#chmod 755 ${HOME}/bin/cmus-lyrics
```

And finally clean up:

```sh
rm cmus-lyrics-master.zip
rm -rf cmus-lyrics-master/
```


### Usage :
Run **cmus-lyrics** and it will fetch and print lyrics of the song currently playing in CMus.


### Credits :
_[Federico Builes] - cmus-lyrics wouldn't have been possible without wonderful [makeitpersonal] created by him._


### License :
[![Public Domain Mark](http://i.creativecommons.org/p/mark/1.0/88x31.png)](http://creativecommons.org/publicdomain/mark/1.0/)  

[perl]:https://www.perl.org
[URI::Escape]:http://search.cpan.org/dist/URI/lib/URI/Escape.pm
[Wget]:https://www.gnu.org/software/wget/
[cmus-lyrics-master.zip]:https://github.com/aswna/cmus-lyrics/archive/master.zip
[CMus]:https://cmus.github.io
[Federico Builes]:https://github.com/febuiles
[makeitpersonal]:https://github.com/febuiles/makeitpersonal
