hoge
---

# setup
```
yum install -y curl git vim openresty mysql memcached redis 
```

# add ssh key
```
curl -L https://gist.githubusercontent.com/doHub1/923ae6402d2342d7f34f57dfabd47b04/raw/588c71029a9bcf9f65b25e1685f75ebcc8165ac9/doWin10.pub >> ~/.ssh/authorized_keys
```


# netdata (Real-time performance monitoring)
## install
```
yum install -y zlib-devel libuuid-devel libmnl-devel gcc make git autoconf autogen automake pkgconfig
git clone https://github.com/firehol/netdata.git --depth=1
cd netdata
sudo ./netdata-installer.sh
systemctl status netdata
```

### OSを再起動しても起動できるようにしておく
```
sudo systemctl enable netdata
```

