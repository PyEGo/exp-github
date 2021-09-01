# exp-github

## Description
Experimental results on Github dataset
## Dataset
Our dataset is available on https://drive.google.com/file/d/1oHr6mbm0d5jIlVxeDkY6iyvow_Q63L_w/view?usp=sharing.<br/>
This repository only provides experimental results.
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
* **GithubTest-me** folder stores DockerizeMe-generated Dockerfile. We config Python3.9 instead of Python2.7.<br/>
  The folder structure is as follow:
```$xslt
.
├── 0
│   └── Dockerfile # DockerizeMe-generated Dockerfile
├── 1
...
└── 99
```
* **GithubTest-reqs** folder stores Pipreqs-generated requirements.txt<br/>
  The folder structure is as follow:
```$xslt
.
├── 0
│   ├── Dockerfile # Template-generated Dockerfile
│   └── requirements.txt # Pipreqs-generated requirements.txt
├── 1
...
└── 99
```
* **Log** folder stores execution logs. 
  We dockerize projects(build docker images and run images in container) based on Dockerfile or requirements.txt,
  and then records execution results into logs.<br/>
  The folder structure is as follow:
```$xslt
.
├── PyEGo.log # log of PyEGo
├── DockerizeMe.log # log of DockerizeMe with Python3.9 interpreter
└── Pipreqs.log # log of Pipreqs with Python3.9 interpreter
```  
* **results_github.csv** stores the result overview of experiments on all projects.

