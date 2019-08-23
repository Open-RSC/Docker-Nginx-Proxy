# Docker Nginx-Proxy

This allows hosting multiple SSL-enabled websites using a Nginx, Lets Encrypt, and Docker.

Based on original guide located at https://blog.ssdnodes.com/blog/host-multiple-ssl-websites-docker-nginx

To ensure a smooth install with all needed components for Open RSC's webserver and to switch from SSH port 22 to port 55555, run the following:

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