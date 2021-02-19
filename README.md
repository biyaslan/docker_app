# Simple Flask App - Docker 

Simple app built on Python Flask.

## Repository Structure 
```
.
├── Dockerfile
├── README.md
├── app
│   ├── requirements.txt
│   └── src
│       ├── server.py
│       └── templates
│           ├── about.html
│           └── index.html
└── docker-compose
    └── docker-compose.yml

4 directories, 7 files
```
## Prerequisites 

* Linux Server

* Python3.8

* Python pip


## Usage

Clone Repository: 

```bash
git clone https://github.com/biyaslan/docker_app.git
```

Change working directory:
```bash
cd docker_app
```

Install requirements:
```bash
pip3 install -r app/requirements.txt
```

Run Application:

```bash
python3.8 app/src/server.py 
```

## Docker Image Build 

Build Image 
```bash
docker image build -t <your-tag> .
```

Push Image
```bash
docker image push <your-image>
```

## Run Docker Container 

Run Container 
```bash
docker container run -d --name sampleapp -p <hostport>:<5000> <your-image>
```

## Docker-Compose

Chage Directory
```
cd docker-compose
```

* NOTE: modify docker-compose.yml file (optional)

Build Image and Run Container 
```
docker-compose up -d --build
```

## Contributing
