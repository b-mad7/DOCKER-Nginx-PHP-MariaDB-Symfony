# NEW SYMFONY PROJECT
- Install Docker
[For Windows](https://docs.docker.com/docker-for-windows/install/) | [For Linux(Ubuntu)](https://docs.docker.com/engine/install/ubuntu/)
- Install PHP
[For Windows](https://www.jeffgeerling.com/blog/2018/installing-php-7-and-composer-on-windows-10) | [For Linux(Ubuntu)](https://linuxize.com/post/how-to-install-php-on-ubuntu-18-04/)
- Install Composer
[For Windows](https://getcomposer.org/download/) | [For Linux(Ubuntu)](https://www.ionos.com/community/hosting/php/install-and-use-php-composer-on-ubuntu-1604/)

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
