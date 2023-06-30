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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1063" class=".btn">#1063</a>
            </td>
            <td>
                <b>
                    fix(test-network): ignore the error output when killing CCAAS containers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi there,

I noticed that when shutting down a test network using `./network.sh down`, the `networkDown()` function will kill the chaincode-as-a-service containers by querying for all containers with name `ccaas`. However, if you did not deploy your chaincode as a service, this `docker kill` command will give an ugly error message as the following:

```
Removing remaining containers
Removing generated chaincode docker images
"docker kill" requires at least 1 argument.
See 'docker kill --help'.

Usage:  docker kill [OPTIONS] CONTAINER [CONTAINER...]

Kill one or more running containers
```

Also, I believe this command is a bit misplaced as it is more logical to have it in `clearContainers()` function. Therefore, I moved the line to the latter function and discarded its stderr (aligned with other clearing container commands).

Thanks

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 02:22:59 +0000 UTC
    </div>
</div>

