# Heroku buildpack: Haskell (WIP)

This is a work in progress, it does not currently work: size restrictions on heroku are making it difficult.

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks)
for Haskell apps. It uses cabal-1.14.0. 

## Usage

    $ ls
    Procfile app.cabal src

    $ heroku create --stack=cedar --buildpack https://github.com/luciferous/heroku-buildpack-haskell.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Haskell app detected
    -----> Building app with cabal
    -----> Running: cabal install

