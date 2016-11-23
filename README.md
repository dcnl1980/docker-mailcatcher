# mailcatcher docker image (works with docker-compose)

It is a very small image (~34 MB uncompressed) available on [docker hub][dockerhubpage] based on [Alpine Linux][alpinehubpage] and using the last available release from the official Github repo of [MailHog][mailhog].

## Usage

Get it:

    git clone https://github.com/dcnl1980/docker-mailcatcher.git

Build it:

    docker-compose build

Run it:

    docker-compose up
    
Then you can send emails from your app to port 1025 and check out the web interface: http://\<your docker host\>:1080/. Or link this container to your webdevelopment container. 

  [mailcatcher]: http://mailcatcher.me/ "MailCatcher fake SMTP server with web interface" 
  [dockerhubpage]: https://hub.docker.com/r/tophfr/mailcatcher/ "Mailcatcher docker hub page"
  [alpinehubpage]: https://hub.docker.com/_/alpine/ "A minimal Docker image based on Alpine Linux with a complete package index and only 5 MB in size!"
