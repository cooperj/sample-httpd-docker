# sample-httpd-docker
Sample project for using the httpd docker container with a dockerfile

I have created this repo with some very basic HTML and a dockerfile to show how a docker can be set up in your code repository.

Let's start by being somewhere easy to access, manage... I like the home folder.

```
cd ~
```

Now we can clone the repo, by using the HTTP connection to GitHub, by using HTTP we can clone it without logging in.

```
git clone https://github.com/cooperj/sample-httpd-docker.git
```

We have now cloned the repo, let's change into its directory.

```
cd sample-httpd-docker
```

We now need to run the command to create an image that can be used to deploy from, remember to use all lowercase in the name you give, the `.` indicates the current directory.

```
sudo docker build -t myproject .
```

That is it, you can launch the project any way you like, here is a sample command.

```
sudo docker run -dit --name sample-site -p 8008:80 mywebsitetest1
```