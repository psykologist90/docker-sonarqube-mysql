# Docker Compose file for Sonarqube with PostGres (Mysql has been deprecated)

## Installation

1. Install docker and docker-compose
1. Clone the repository
1. Open terminal and cd into ./sonarqube-postgres
1. Run `docker-compose up -d`
1. Open browser and browse to <http://youripaddress:9000/>

## Complete installation instructions for Ubuntu

### Docker

I.e. with convenience script:

```bash
curl -fsSL get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

> <https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/>

### Sonarqube with MySQL

```bash
// Clone repository
sudo apt-get install git
git clone https://github.com/psykologist90/docker-sonarqube-db.git

// Start docker-compose
cd docker-sonarqube-db/sonarqube-postgres
echo 'PG_PASS=thepassyouwant' > .env
docker-compose up -d
```