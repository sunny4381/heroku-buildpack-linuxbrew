Heroku buildpack: linuxbrew
=======================

You can install any packages by using [linuxbrew](https://github.com/Homebrew/linuxbrew).

Usage
-----
To use this buildpack, you should prepare a .buildpacks file that contains this buildpack url and your real buildpack url:

    $ ls
    .celler
    .buildpacks
    ...

    $ cat .celler
    mecab
    mecab-ipadic
    
    $ cat .buildpacks
    https://github.com/sunny4381/heroku-buildpack-linuxbrew

    $ heroku create --buildpack https://github.com/ddollar/heroku-buildpack-multi

    $ git push heroku master
    ...

License
----
MIT
