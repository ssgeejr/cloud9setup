# cloud9setup
compiled and tested list of scripts that allow a person to use cloud9 on an existing AWS instance 

#Amazon internal CIDR for connectivity
```
18.188.9.0/27
18.188.9.32/27
```

# as root (these should already be done at the system level 
```
sudo yum groupinstall -y development
sudo yum install glibc-static
```

# As the user needing to run cloud9
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
. ~/.nvm/nvm.sh
nvm install node
node -e "console.log('Running Node.js ' + process.version)"
curl -L https://raw.githubusercontent.com/c9/install/master/install.sh | bash
```
