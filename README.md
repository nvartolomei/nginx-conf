# NGINX-Conf

A collection of must-have nginx configuration snippets, carefully crafted and
tested, intended for personal use, you'd better check [Michael Goreanski](https://github.com/Umkus/nginx-boilerplate)'s nginx-boilerplate project.

## Install
Clone this repository to nginx configuration prefix directory (usually `/usr/local/nginx/conf`).

    cd /usr/local/nginx/conf
    git clone git@github.com:nvartolomei/nginx-conf.git

Cool, from this point you can include any snippet provided by nginx-conf in your
`nginx.conf` file.

For example `nginx.conf` may look like this:

    events {
        include    nginx-conf/system/connections.conf;
    }

    http {
        # ./sites/ is where your configurations for sites lives
        include    sites/*.conf;
    }

#### Colophon
Thanks to...

* [Michael Goreanski](https://github.com/Umkus/nginx-boilerplate) for solid nginx configuration base
