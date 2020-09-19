# NEW SYMFONY PROJECT
- Install Docker
[For Windows](https://docs.docker.com/docker-for-windows/install/) | [For Linux(Ubuntu)](https://docs.docker.com/engine/install/ubuntu/)
- Install PHP
- Install Composer
[Composer](https://getcomposer.org/download/)

```bash
docker-compose up -d
```

```bash
composer create-project symfony/website-skeleton src
```

## On UBUNTU server
If needed install php xml extension
```bash
apt-get install php7.2-xml
```

* If it fails with: "proc_open(): fork failed - Cannot allocate memory"
Check free memory
```bash
free -m
```
Then increase memory to 1024
```bash
sudo /bin/dd if=/dev/zero of=/var/swap.1 bs=1M count=1024
sudo /sbin/mkswap /var/swap.1
sudo /sbin/swapon /var/swap.1
```
