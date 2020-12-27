# Install go language on Raspberry Pi

To install go for the ARM Arquitecture used on the Raspberry Pi, look for the ARM v6 version of the install file on [GoLang.org](https://golang.org/dl/)

At the time of this writing the file for the current version was ***go1.15.6.linux-armv6l.tar.gz***

After downloading the file you can do the installation by running the following command:
```
# Substitute the tar.gz file name for the file you downloaded from https://golang.org/dl/
sudo tar -C /usr/local -xzf ~/Downloads/go1.15.6.linux-armv6l.tar.gz 
```

Add the following line of code to your ~/.profile file:
```
export PATH=$PATH:/usr/local/go/bin
```

You can put the export into the file ~/etc/profile instead to make go compiler accesible from any user.

Verify your go installation is running properly:
```
# We do the export manually this time, since you probably are still in the same terminal and haven't run the profile script you just modified.
export PATH=$PATH:/usr/local/go/bin

# If go install was succesful then this command will show the go version you just installed.
go version
```
