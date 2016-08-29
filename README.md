#Docker image on Centos:7 to run NetAcuity 

#Create container
```
docker run -i -t -d --name=NetAcuity -h=NetAcuity -p 5001:80 -p 5002:22 -p 5400:5400 cristo/netacuity
```

#SSH
```
ssh -p5002 root@localhost
password: root
```

#Test NetAcuity availability to run on this machine.
```
cd /home && ./NATest.bin
```

# etcKeeper 
Added etcKeeper - autocommit on exit to /etc git local repository

#Origin
[Docker Hub] (https://hub.docker.com/r/cristo/netacuity)

[BitBucket] (https://bitbucket.org/monte-fm/netacuity)