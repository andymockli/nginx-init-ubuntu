nginx-init-ubuntu install template flavors
=================


## Ubuntu /etc/nginx/sites-enabled
For example, if your install looked something like this

    # ...[snip]
    ./configure --prefix=/etc/nginx --sbin-path=/usr/sbin/nginx --conf-path=/etc/nginx/nginx.conf --pid-path=/run/nginx.pid --error-log-path=/var/log/nginx/error.log --http-log-path=/var/log/nginx/access.log --user=www-data --group=www-data
    make
    sudo make install
    
    #copy/download/curl/wget the init script
    sudo wget https://raw.githubusercontent.com/JasonGiedymin/nginx-init-ubuntu/master/nginx -O /etc/init.d/nginx
    sudo chmod +x /etc/init.d/nginx

    # ...[snip]

Then just also do this

    sudo wget https://raw.githubusercontent.com/JasonGiedymin/nginx-init-ubuntu/master/defaults/ubuntu-sites-enabled-defaults -O /etc/default/nginx
    sudo chmod +x /etc/default/nginx

