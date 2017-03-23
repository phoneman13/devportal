---
title: Choose Library
position: 1
---

Getting started to develop robust and feature rich **steem** applications couldn't be easier. Accessing
steem data is easy from various options depending on your infrastructure and objectives. 

Building a picture discovery app is a breeze with the javascript library. 
Running a steemd instance would open full access to the steem wallet and mining capabilities. 

##### **Javascript Developers**

Our official JS toolkit is located at : [https://github.com/steemit/steem-js](https://github.com/steemit/steem-js)

The Javascript library let's your app easily access steem blockchain data and also perform
user actions. 

Documentation to get going is located in the [Javascript Section](#javascriptgetting_started).

##### **steemd**

The simplest way to get started is by deploying a prebuilt dockerized container. 
 
##### Dockerized p2p Node
*To run a p2p node (ca. 2GB of memory is required at the moment):*
```
docker run \
    -d -p 2001:2001 -p 8090:8090 --name steemd-default \
    steemit/steem

docker logs -f steemd-default  # follow along
```

##### Dockerized Full Node
*to run a node with all the data (e.g. for supporting a content website) that uses ca. 14GB of memory and growing:*
```
docker run \
    --env USE_WAY_TOO_MUCH_RAM=1 \
    -d -p 2001:2001 -p 8090:8090 --name steemd-full \
    steemit/steem

docker logs -f steemd-full
```