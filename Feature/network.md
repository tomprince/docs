# Network

By default, Hyper\_ setup a Layer-2 virtual private network for every user. All containers of a user will be automatically placed in the user's own network. Containers in the same network are reachable to each other, but isolated from other networks. Also, containers are able to access the Internet, but not accessible from Internet (To enable the public access, you can associate [floating IP](./fip.md) to container).

The [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing) of the default private network is set to `172.16.0.0/16`. Note: Hyper\_ reserves a few addresses for its own usage. When a new container is launched, Hyper\_ will automatically assign a private IP address to the container. Currently, there is no way to control the IP allocation.


