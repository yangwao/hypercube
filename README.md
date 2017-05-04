# hypercube
aarch64 docker images for decentralized services soon™
roadmap
 * scuttlebutt ([staltz/easy-ssb-pub](https://github.com/staltz/easy-ssb-pub))
 * ipfs
 * bitcoin-core
 
# how to run on AARCH64

```
apt-get install docker.io
docker run -e "PUB_URL=ssb.kic9832227.hypersignal.xyz" -v $HOME/.ssb:/root/.ssb -p 80:80 -p 8008:8008 -p 8007:8007 --restart=unless-stopped --name ssb-pub -d yangwao/easy-ssb-pub-aarch64
```

# easy-ssb docker image
```
git clone https://github.com/staltz/easy-ssb-pub
docker-compose build
docker images 
docker tag b40fe3b167aa yangwao/easy-ssb-pub-aarch64
docker push yangwao/easy-ssb-pub-aarch64
```

