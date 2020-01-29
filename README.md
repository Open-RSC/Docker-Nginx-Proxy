# Docker Nginx-Proxy

This allows proxying for hosting multiple SSL-enabled websites using a Nginx and Docker.

Based on original guide located at https://blog.ssdnodes.com/blog/host-multiple-ssl-websites-docker-nginx

Ensure that multiple domain covering SSL cert files "default.crt" and "default.key" are placed in the "certs" folder.

```
sudo make install
```

When first set up, ensure the following has been ran if you have not used the install script:

```
sudo docker network create nginx-proxy
```

When ready, utilize:

```
sudo make start
```

To see the current status of the docker-compose containers:

```
sudo make logs
```
