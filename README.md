# workspace-centos7-jdk8
```
git clone https://github.com/nojaja/workspace-centos7-jdk8.git
docker build -t workspace-centos7-jdk8:1.0 .

$ docker images
  # REPOSITORY              TAG                 IMAGE ID            CREATED              VIRTUAL SIZE
  workspace-centos7-jdk8   1.0       30822b930a81   About a minute ago   894MB

docker run -it --rm -p 22:22 -v %CD%:/root/workspace workspace-centos7-jdk8:1.0
```
# vscode

`C:\Users\{username}\.ssh\config`
を編集
```
Host workspace-centos7-jdk8-2
    HostName localhost
    Port 22
    User root
````
Remote-SSHにて接続
