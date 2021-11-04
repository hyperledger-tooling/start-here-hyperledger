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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/528" class=".btn">#528</a>
            </td>
            <td>
                <b>
                    Add an option to stage docker images locally to KIND
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses a compromise for development workflows requiring different patterns for loading images into the KIND / kubernetes cluster. 

- For casual / default usage, the docker images are loaded from the public container registries (docker.io and ghcr.io)

- For developers with network issues connecting to public registries, this PR allows for an offline "pull" and stage to the KIND control plane: 
```
export TEST_NETWORK_STAGE_DOCKER_IMAGES=true
./network kind     # << this will pull from the public repos, and run kind load docker-image ...  

./network up 
```

- For test/development of the CI latest build outputs, the container registry and revision can be overridden: 
```
export TEST_NETWORK_FABRIC_VERSION=amd64-latest 
export TEST_NETWORK_FABRIC_CA_VERSION=amd64-latest 
export TEST_NETWORK_FABRIC_CONTAINER_REGISTRY=hyperledger-fabric.jfrog.io

./network up 
```

- For active development of core Fabric images (e.g. peer, orderer), the KIND control plane can be directly loaded with local builds: 
```
make docker # (in fabric) 

export TEST_NETWORK_FABRIC_VERSION=2.4.0 

./network load-images 
./network up 
``` 


@mbwhite and @SamYuan1990 can you please give this PR a test run to double-check that it meets your target use cases?   Matthew I had some difficulty testing out PR #507 and the `candidate-use-builtin-ccs-builder` branch with the mainline network scripts.  I think this is a better fit for that workflow. 


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:57:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    Use built-in Peer chaincode-as-a-server builder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using the variant of the peer's docker container from https://github.com/hyperledger/fabric/pull/2990  this PR adapts the K8S deployment to use this inbuilt chaincode builder.

- creates two deployments of the chaincode for each peer
- uses the builders ability to template the fields in the connection.json

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 10:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/523" class=".btn">#523</a>
            </td>
            <td>
                <b>
                    Updated logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - updated the logging for the application command; wasn't very good
- added some information to the help option. the current settings
  useful if you're not sure what you've set


FYI @jkneubuh 

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 09:29:47 +0000 UTC
    </div>
</div>

