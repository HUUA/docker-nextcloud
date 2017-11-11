[![Docker Nextcloud](https://raw.githubusercontent.com/crazy-max/docker-nextcloud/master/res/docker-nextcloud.png)](https://github.com/crazy-max/docker-nextcloud)

[![Version](https://images.microbadger.com/badges/version/crazymax/nextcloud.svg?style=flat-square)](https://microbadger.com/images/crazymax/nextcloud)
[![Docker Build Status](https://img.shields.io/docker/build/crazymax/nextcloud.svg?style=flat-square)](https://hub.docker.com/r/crazymax/nextcloud/)
[![Docker Stars](https://img.shields.io/docker/stars/crazymax/nextcloud.svg?style=flat-square)](https://hub.docker.com/r/crazymax/nextcloud/)
[![Docker Pulls](https://img.shields.io/docker/pulls/crazymax/nextcloud.svg?style=flat-square)](https://hub.docker.com/r/crazymax/nextcloud/)
[![Docker Build](https://img.shields.io/docker/automated/crazymax/nextcloud.svg?style=flat-square)](https://hub.docker.com/r/crazymax/nextcloud/)
[![Nextcloud Version](https://img.shields.io/badge/nextcloud-12.0.3-green.svg?style=flat-square)](https://nextcloud.com)
[![Donate Paypal](https://img.shields.io/badge/donate-paypal-7057ff.svg?style=flat-square)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ADCA2SNLJ9FW4)

## About

🐳 [Nextcloud](https://nextcloud.com) Docker image based on Nextcloud ☁ stable image with advanced features. More information about the based Nextcloud image on the [official repository](https://github.com/nextcloud/docker).

## Features

### Included

* [SSMTP](https://github.com/alterrebe/docker-mail-relay) for SMTP relay (use PHP as send mode on Nextcloud)
* Cron for Nextcloud background jobs

### From docker-compose

* Reverse proxy with [nginx-proxy](https://github.com/jwilder/nginx-proxy)
* Creation/renewal of Let's Encrypt certificates automatically with [letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion)
* [Redis](https://github.com/docker-library/redis) for caching

## Use this image

Download the [docker-compose.yml](docker-compose.yml) template and the [env](env) folder in the same directory.<br />
Edit those files with your preferences, then run :

```bash
$ docker-compose up -d
```

Do not forget to choose **Cron** as background jobs :

![Background jobs](https://raw.githubusercontent.com/crazy-max/docker-nextcloud/master/res/background-jobs.png)

And you can customize the **Email server** settings with your preferences :

![Email server](https://raw.githubusercontent.com/crazy-max/docker-nextcloud/master/res/email-server.png)

## How can i help ?

We welcome all kinds of contributions :raised_hands:!<br />
The most basic way to show your support is to star :star2: the project, or to raise issues :speech_balloon:<br />
Any funds donated will be used to help further development on this project! :gift_heart:

[![Donate Paypal](https://github.com/crazy-max/docker-nextcloud/blob/master/res/paypal.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ADCA2SNLJ9FW4)

## License

MIT. See `LICENSE` for more details.
