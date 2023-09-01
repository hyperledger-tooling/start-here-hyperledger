---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1085" class=".btn">#1085</a>
            </td>
            <td>
                <b>
                    Fix OrdererEndpoints in test-network's bft sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch fixes the description of orderer2-4 in OrdererEndpoints in test-network's bft-config/configtx.yaml.

### Details
I noticed that the current configuration in the configtx.yaml file lists all endpoints under "orderer.example.com" with different port numbers. I wonder if the orderer names should be distinct, such as 'orderer2.example.com', 'orderer3.example.com', and 'orderer4.example.com', each with their respective port numbers.

#### Check for problems and their fixes 

I commented out the first entry of orderer.example.com:7050 temporarily to see if peers have trouble pulling blocks from the other endpoints as shown in the following log.

```bash
$ docker logs peer0.org1.example.com
...
2023-08-29 05:12:55.161 UTC 005b WARN [peer.blocksprovider] DeliverBlocks -> Could not connect to ordering service: could not dial endpoint 'orderer.example.com:7056': failed to create new connection: connection error: desc = "transport: error while dialing: dial tcp 172.20.0.7:7056: connect: connection refused" channel=mychannel
2023-08-29 05:12:55.161 UTC 005c WARN [peer.blocksprovider] DeliverBlocks -> Disconnected from ordering service. Attempt to re-connect in 4.6s channel=mychannel
```

After that, I tested by fixing the hostname of orderer2-4 and validated that fix solves the problem as shown in the following log.

```bash
$ docker logs peer0.org1.example.com
...
2023-08-29 05:18:35.155 UTC 0031 INFO [peer.blocksprovider] Start -> BlockReceiver starting channel=mychannel orderer-address=orderer2.example.com:7052
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 08:27:55 +0000 UTC
    </div>
</div>

