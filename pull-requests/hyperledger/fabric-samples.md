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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/519" class=".btn">#519</a>
            </td>
            <td>
                <b>
                    nit fixs for test network k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. busybox latest image tag
2. pull images with more images
3. load images to kind cluster at local

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 16:07:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/518" class=".btn">#518</a>
            </td>
            <td>
                <b>
                    Allow overrides of the docker registry for fabric images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The test-network-k8s had some cruft related to a build/edit/test workflow revolving around the KIND image plane to load docker Images into the cluster.  This change allows users to update the remote docker registry and run Fabric with: 

- The latest CI/CD images.  E.g.: 
```
export TEST_NETWORK_FABRIC_CA_VERSION="amd64-latest"
export TEST_NETWORK_FABRIC_CONTAINER_REGISTRY="hyperledger-fabric.jfrog.io"
export TEST_NETWORK_FABRIC_VERSION="amd64-latest"

./network up 
``` 


- Custom images created on a local workstation.  E.g.: 
```
fabric $ make docker 
fabric $ docker tag hyperledger/fabric-peer localhost:5000/hyperledger/fabic-peer:my-fancy-tag 
fabric $ docker push localhost:5000/hyperledger/fabric-peer:my-fancy-tag
...

test-network-k8s $ export TEST_NETWORK_FABRIC_CONTAINER_REGISTRY=localhost:5000/hyperledger 
test-network-k8s $ export TEST_NETWORK_FABRIC_VERSION=my-fancy-tag 

./network up 
```

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 11:42:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/516" class=".btn">#516</a>
            </td>
            <td>
                <b>
                    test-network: Make the regexp of checking version more strict (backpo…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                (Backport #515)

Make the regular expression of checking version more strict in `test-network/network.sh` for comparing only the main version.

If the version string (by `'peer version'`) includes other "Version: " strings, the comparing version between `LOCAL_VERSION` and `DOCKER_IMAGE_VERSION` would be failed because of the cropping by '`head -1`'.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 12:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/515" class=".btn">#515</a>
            </td>
            <td>
                <b>
                    test-network: Make the regexp of checking version more strict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the regular expression of checking version more strict in `test-network/network.sh` for comparing only the main version.

If the version string (by `'peer version'`) includes other "Version: " strings, the comparing version between `LOCAL_VERSION` and `DOCKER_IMAGE_VERSION` would be failed because of the cropping by '`head -1`'.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 10:01:46 +0000 UTC
    </div>
</div>

