# Thaliyola

## URL : https://thaliyola.herokuapp.com/

# How To Install Go 1.12 on Ubuntu and host in heroku <br>
Go is an open source programming language developed by a team at Google.<br>

# Step 1 <br>
  `sudo apt-get update`

# Step 2 <br>
download the Go language binary archive file <br>
 `wget https://dl.google.com/go/go1.12.7.linux-amd64.tar.gz` <br>

# Step 3 <br>
extract the downloaded archive and install it <br>
   `sudo tar -xvf go1.12.7.linux-amd64.tar.gz` <br>
   `sudo mv go /usr/local `  <br>
   
# Step 4 : Setup Go Environment <br>
Now you need to setup Go language environment variables for your project.<br>
Commonly you need to set 3 environment variables as GOROOT, GOPATH and PATH.<br>

GOROOT is the location where Go package is installed on your system. <br>

   `export GOROOT=/usr/local/go ` <br>

GOPATH is the location of your work directory. For example my project directory is ~/Developer/thaliyola<br>

   `export GOPATH=$HOME/Developer/thaliyola<br>`

Now set the PATH variable to access go binary system wide.<br>

   `export PATH=$GOPATH/bin:$GOROOT/bin:$PATH<br> `
   
All the above environment will be set for your current session only. To make it permanent add above commands in ~/.profile file.<br>

# Step 5 – Verify Installation<br>
At this step, you have successfully installed and configured go language on your system. First, use the following command to check the Go version.<br>

   `go version `<br>
   
   go version go1.12.7 linux/amd64<br>
Now also verify all configured environment variables using following command.<br>
#----------------------------------------------------------------------------------------------------
Link : heroku.com  and create account. <br>
   https://github.com/heroku/heroku-buildpack-go  <br>
   https://devcenter.heroku.com/articles/getting-started-with-go <br>

# heroku log

 `jithu@jithu-PC-LL750CS6R:~/developer$ heroku logs --tail --app thaliyola`








