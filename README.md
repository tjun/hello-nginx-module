# hello-nginx-module

## build

    wget http://nginx.org/download/nginx-1.7.9.tar.gz
    git clone git@github.com:tjun/hello-nginx-module.git
    tar zxf nginx-1.7.9
    cd nginx-1.7.9
    ./configure --add-module=../hello-nginx-module/
    make
    sudo make install

## config

add config to nginx.conf

    location /hello {
      nginx_hello;
    }


