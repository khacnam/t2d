Before following and using this script, go through this [video](https://www.youtube.com/watch?v=m4jm2ZOA9bg). In this video tutorial I demonstrated how to use t2d script.

> At the start of the video, I used few curl commands to download the t2dscript, for your purpose, I made a seperate script. So your intial download command is different.

The below mentioned 3 commnds will initiate the installation process of dokku and Forem. So before using this script, I would suggest you to go through the above mentioned video.
```
wget https://raw.githubusercontent.com/khacnam/t2d/main/t2d.sh
chmod +x t2d.sh
./t2d.sh
```


## Must do before using the script

1. First make sure that you point out subdomain/domain properly via your DNS providor. Failure of this might result in build fail beacause it the script might not be able to use get you a free SSL certificate using letsencrypt which is a madatory.
2. Go to [honeybadger](https://www.honeybadger.io/) website and create a free account and generate your api key. Which will be used during the installation process
3. During the initial setup, it might take upto 30-40 minutes install, so have some patience and gop through the logs.

## During installation

1. During the installation, first the script will install dokku. So after the installation of dokku, rather than directly moving to the next step go visit you IP address and finish dokku instllation via browser. If this is not done, someone else can visit your IP adress and can have access to your server.
2. Wile setting up dokku via browser, it would be preferable to change the default vhost to IP:PORT format.

> For more info regarding this, go throgh this [video tutorial](https://www.youtube.com/watch?v=m4jm2ZOA9bg), where I use t2d script to install Forem from scratch. You can skip to the dokku configuration part
