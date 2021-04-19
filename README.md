# exp-github

## Description
Experimental results on Github dataset
## Dataset
Our dataset is available on https://drive.google.com/file/d/1oHr6mbm0d5jIlVxeDkY6iyvow_Q63L_w/view.<br/>
This repository only provides experiment results.
## Architecture
* **GithubTest-ego** folder stores PyEGo-generated Dockerfile.<br/>
  The folder structure is as follow:
```$xslt
.
├── 0
│   └── Dockerfile # PyEGo-generated Dockerfile
├── 1
...
└── 99
```
* **GithubTest-me-<3.8 or 3.9>** folder stores DockerizeMe-generated Dockerfile. We revise first command "FROM python:2.7.13"
  to "FROM python:3.8" or "FROM python:3.9".<br/>
  The folder structure is as follow:
```$xslt
.
├── 0
│   └── Dockerfile # DockerizeMe-generated Dockerfile (Differ in "FROM python:3.8" and "FROM python:3.9")
├── 1
...
└── 99
```
* **GithubTest-reqs-<3.8 or 3.9>** folders stores Pipreqs-generated requirements.txt<br/>
  The folder structure is as follow:
```$xslt
.
├── 0
│   ├── Dockerfile # Template-generated Dockerfile (Differ in "FROM python:3.8" and "FROM python:3.9")
│   └── requirements.txt # Pipreqs-generated requirements.txt
├── 1
...
└── 99
```
* **Log** folder stores execution logs. 
  We dockerize projects(build docker images and run images in container) based on PyEGo-generated Dockerfile, DockerizeMe-generated Dockerfile or Pipreqs-generated requirements.txt,
  and then records execution results into logs.<br/>
  The folder structure is as follow:
```$xslt
.
├── PyEGo.log # log of PyEGo
├── DockerizeMe-3.8.log # log of DockerizeMe with Python3.8 interpreter
├── DockerizeMe-3.9.log # log of DockerizeMe with Python3.9 interpreter
├── Pipreqs-3.8.log # log of Pipreqs with Python3.8 interpreter
└── Pipreqs-3.9.log # log of Pipreqs with Python3.9 interpreter
```  
* **results_github.csv** stores the result overview of experiments on all projects.

