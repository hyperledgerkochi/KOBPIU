# Installing the SDK
### Release channels
The Indy SDK release process defines the following release channels:

* `master` - development builds for each push to master branch.
* `rc` - release candidates.
* `stable` - stable releases.
### Ubuntu based distributions (Ubuntu 20.04)
It is recommended to install the SDK packages with APT:

    ```sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys CE7709D068DB5E88
    sudo add-apt-repository "deb https://repo.sovrin.org/sdk/deb xenial stable"
    sudo apt-get update
    sudo apt-get install -y libindy
    ```

# Starting local pools using Docker
First you have to clone the hyperledger indy sdk repository.
```git clone https://github.com/hyperledger/indy-sdk.git
```
In the indy-sdk folder open a terminal. Run the commands
```docker network create --subnet 10.0.0.0/8 indy_pool_network
docker build --build-arg pool_ip=10.0.0.2 -f ci/indy-pool.dockerfile -t indy_pool .
docker run -d --ip="10.0.0.2" --net=indy_pool_network indy_pool
```
#Indy-Cli
Indy-Cli is the command line interface where we can interact with pools, wallets and DIDs.
###Installing Indy-Cli
``` sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys CE7709D068DB5E88
    sudo add-apt-repository "deb https://repo.sovrin.org/sdk/deb xenial stable"
    sudo apt-get update
    sudo apt-get install -y indy-cli
```



