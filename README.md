# Useful Linux Command
Some linux commands I found are usefule when I managed our system.

## Change CUDA Version

```
export PATH=/usr/local/cuda-11.8/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/cuda-11.8/lib64:$LD_LIBRARY_PATH
```

## Passwordless SSH Login 

On your computer, run
```
ssh-keygen
```
You will see `.pub` file on your computer. Then upload the public key to the host by the following code
```
ssh-copy-ide [remote_username]@[server_ip_address]
```
Or this on Windows
```
type $env:USERPROFILE\.ssh\id_rsa.pub | ssh [remote_username]@[server_ip_address] "cat >> .ssh/authorized_keys"
```


## Conda
### Remove environment
```
conda remove --name myenv --all
```

## Memory Usage
### Memory Usage of Each folder
```
du -h --max-depth=1
```

## Create Account
```
sudo adduser new_user
sudo mkdir /data/new_user 
sudo chown new_user:new_user  /data/new_user 
```


## Go to iCloud Drive
access iCloud drive on Mac in terminal
```
cd ~/Library/Mobile\ Documents/com~apple~CloudDocs
```

