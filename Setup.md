# Starting local pools using Docker
First you have to clone the hyperledger indy sdk repository.
```
git clone https://github.com/hyperledger/indy-sdk.git

```
In the indy-sdk folder open a terminal. Run the commands
```
docker network create --subnet 10.0.0.0/8 indy_pool_network
docker build --build-arg pool_ip=10.0.0.2 -f ci/indy-pool.dockerfile -t indy_pool .
docker run -d --ip="10.0.0.2" --net=indy_pool_network indy_pool

```

