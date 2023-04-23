# S3-Connect
S3 Connection with Rclone and winfsp with local mount

1. Download ---> Winfsp  ---> Windows Mount as Drive ---> https://github.com/billziss-gh/winfsp/releases

2a. Rclone  ---> Rclone ---> OpenSource Cli tools for almost all cloud storages ---> https://rclone.org/downloads/

2b. GIT Bash ---> https://git-scm.com/downloads

3. Create s3 bucket

#######################################################################################################
4. mkdir /c/rclone

cd /c/rclone && curl -# -LO https://downloads.rclone.org/v1.53.3/rclone-v1.53.3-windows-amd64.zip

unzip rclone-v1.53.3-windows-amd64.zip

cd rclone-v1.53.3-windows-amd64

./rclone.exe config

./rclone  mount cloudgeeks-ca:/ S: --vfs-cache-mode full -vv


rclone  mount Cherry:/ O: --vfs-cache-mode full -vv --drive-shared-with-me
