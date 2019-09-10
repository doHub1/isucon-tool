hoge
---

# setup
```
yum install -y curl git vim openresty mysql memcached redis 
```

# add ssh key
```
curl -L https://raw.githubusercontent.com/doHub1/gh-pages/master/key.pub >> ~/.ssh/authorized_key
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

