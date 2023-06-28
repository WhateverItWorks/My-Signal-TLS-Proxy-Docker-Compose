# Signal TLS Proxy
Help people in Iran reconnect to Signal

### Install Certbot
```
sudo apt install python3-certbot-nginx
```

To run a Signal TLS proxy, you will need a host that has ports 80 and 443 available and a domain name that points to that host.

``` https://signal.org/blog/run-a-proxy/ ```

Your proxy is now running! You can share this with the URL `https://signal.tube/#<your_host_name>`

## Updating from a previous version

If you've previously run a proxy, please update to the most recent version by pulling the most recent changes from `main`, then restarting your Docker containers:

```
docker-compose down
docker-compose pull
docker-compose up -d
```

### Advanced

- [Enable Google TCP BBR](https://www.linuxbabe.com/ubuntu/enable-google-tcp-bbr-ubuntu)
