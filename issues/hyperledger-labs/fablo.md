---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fablo/issues/434" class=".btn">434</a>
            </td>
            <td>
                <b>
                    "Error while dialing" when using CouchDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span>
            </td>
            <td>
                Hey, I have a network with 3 orgs and single peer that works perfectly when using LevelDb as option in the `fablo-config.json` file. However, when I change to CouchDb I start having this error:

```
============ 😻 Creating 'my-channel1' on supplier/peer0 😻 ==============
Creating channel with name: my-channel1
   Orderer: orderer0.group1.orderer.supplychain.com:7030
   CORE_PEER_LOCALMSPID: supplierMSP
   CORE_PEER_ADDRESS: peer0.supplier.supplychain.com:7041
   CORE_PEER_MSPCONFIGPATH: /var/hyperledger/cli/crypto/users/Admin@supplier.supplychain.com/msp
2024-03-29 15:55:44.237 UTC 0001 INFO [channelCmd] InitCmdFactory -> Endorser and orderer connections initialized
2024-03-29 15:55:44.350 UTC 0002 INFO [cli.common] readBlock -> Received block: 0
Error: error getting endorser client for channel: endorser client failed to connect to peer0.supplier.supplychain.com:7041: failed to create new connection: connection error: desc = "transport: error while dialing: dial tcp 172.24.0.6:7041: connect: connection refused"
```

I found a few similar issues but the solutions didn't work for me. I'm running Linux on a VM, but I have enough RAM so this isn't the problem. Also, all containers are running. This is my `docker ps -a` output:

```
CONTAINER ID   IMAGE                              COMMAND                  CREATED         STATUS         PORTS                                                                                            NAMES
24ea940fb135   hyperledger/fabric-tools:2.5.6     "/bin/bash"              6 minutes ago   Up 6 minutes                                                                                                    cli.orderer.supplychain.com
0d4c3f6a7aba   hyperledger/fabric-ca:1.5.5        "sh -c 'fabric-ca-se…"   6 minutes ago   Up 6 minutes   0.0.0.0:7080->7054/tcp, :::7080->7054/tcp                                                        ca.retailer.supplychain.com
4b5f09b906f1   hyperledger/fabric-tools:2.5.6     "/bin/bash"              6 minutes ago   Up 6 minutes                                                                                                    cli.retailer.supplychain.com
ff44240c51da   hyperledger/fabric-tools:2.5.6     "/bin/bash"              6 minutes ago   Up 6 minutes                                                                                                    cli.distributor.supplychain.com
29b854ba5ce8   hyperledger/fabric-peer:2.5.6      "peer node start"        6 minutes ago   Up 6 minutes   7051/tcp, 0.0.0.0:7061->7061/tcp, :::7061->7061/tcp, 0.0.0.0:8061->9440/tcp, :::8061->9440/tcp   peer0.distributor.supplychain.com
baeef946931f   couchdb:3.1                        "tini -- /docker-ent…"   6 minutes ago   Up 6 minutes   4369/tcp, 9100/tcp, 0.0.0.0:5140->5984/tcp, :::5140->5984/tcp                                    couchdb.peer0.retailer.supplychain.com
50a001fd0c38   hyperledger/fabric-tools:2.5.6     "/bin/bash"              6 minutes ago   Up 6 minutes                                                                                                    cli.supplier.supplychain.com
03564565be4f   hyperledger/fabric-orderer:2.5.6   "orderer"                6 minutes ago   Up 6 minutes   0.0.0.0:7030->7030/tcp, :::7030->7030/tcp, 7050/tcp, 0.0.0.0:8030->9440/tcp, :::8030->9440/tcp   orderer0.group1.orderer.supplychain.com
400f88004d32   hyperledger/fabric-ca:1.5.5        "sh -c 'fabric-ca-se…"   6 minutes ago   Up 6 minutes   0.0.0.0:7020->7054/tcp, :::7020->7054/tcp                                                        ca.orderer.supplychain.com
402e8df45eb1   hyperledger/fabric-ca:1.5.5        "sh -c 'fabric-ca-se…"   6 minutes ago   Up 6 minutes   0.0.0.0:7060->7054/tcp, :::7060->7054/tcp                                                        ca.distributor.supplychain.com
908f8cf9a9da   couchdb:3.1                        "tini -- /docker-ent…"   6 minutes ago   Up 6 minutes   4369/tcp, 9100/tcp, 0.0.0.0:5100->5984/tcp, :::5100->5984/tcp                                    couchdb.peer0.supplier.supplychain.com
44f2ac7e4229   couchdb:3.1                        "tini -- /docker-ent…"   6 minutes ago   Up 6 minutes   4369/tcp, 9100/tcp, 0.0.0.0:5120->5984/tcp, :::5120->5984/tcp                                    couchdb.peer0.distributor.supplychain.com
874e6ad9eaa7   hyperledger/fabric-peer:2.5.6      "peer node start"        6 minutes ago   Up 6 minutes   0.0.0.0:7041->7041/tcp, :::7041->7041/tcp, 7051/tcp, 0.0.0.0:8041->9440/tcp, :::8041->9440/tcp   peer0.supplier.supplychain.com
a2c9c789ca24   hyperledger/fabric-peer:2.5.6      "peer node start"        6 minutes ago   Up 6 minutes   7051/tcp, 0.0.0.0:7081->7081/tcp, :::7081->7081/tcp, 0.0.0.0:8081->9440/tcp, :::8081->9440/tcp   peer0.retailer.supplychain.com
46b648db1a6a   hyperledger/fabric-ca:1.5.5        "sh -c 'fabric-ca-se…"   6 minutes ago   Up 6 minutes   0.0.0.0:7040->7054/tcp, :::7040->7054/tcp                                                        ca.supplier.supplychain.com
```

I really appreciate any help!

Edit: Sometimes it works correctly when I do `fablo recreate`, but it's really inconsistent. Also, most of the times I do `fablo reset` it fails again, so I need to fix this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-29 16:03:14 +0000 UTC
    </div>
</div>

