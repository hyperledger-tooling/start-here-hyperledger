---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Push to right place
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 18:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Update token
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 18:08:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Test PR 1 build at labs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 17:45:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Switch from Host OS ingress to EXTERNAL-IP ingress for internal traffic - READY FOR MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR: 

- Switches to a CLUSTER-IP network interface for communication with the K8s Ingress

- Adds configuration notes for EKS and IKS clusters 

- Adds a `M.E.L.V.I.N.` ("Cousin of MARVIN") style end-to-end test, including chaincode deployments for `ccaas` and `k8s` executors on a scratch / disposable KIND cluster.

With the previous configuration, the network domain was based on the HOST OS interface to route traffic through the ingress controller.  This was _extremely confusing_, as the network IP varied widely from environment to environment.  With the new scheme, pods communicate with the ingress controller via the Kube INTERNAL (CLUSTER_IP) interface, which does not require a route back to the host OS.

The resulting configuration / README / guidelines are _tremendously simplified_, as the cluster IP is readily available to both the setup scripts and the pods running in Kubernetes.

Tested on the following environments - all more or less ... _just work_:

- [X] EKS
- [X] IKS
- [X] KIND + OSX
- [X] WSL2
- [X] vagrant + fabric-devenv
- [X] Fyre : (peer lcient on fyre, localho,st ingress)
- [X] Fyre : (peer client on fyre, public DNS)
- [X] Fyre : peer client on localhost, remote kube at Fyre + public DNS
- [X] Rancher + moby
- [X] Rancher + containerd / nerdctl

👍 👍 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-11 20:27:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Amazon EKS configuration guidelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 18:06:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Feature/rancher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds README notes on sample-network configurations for [Rancher Desktop](https://rancherdesktop.io) clusters and the vagrant-based [fabric-devenv](https://github.com/hyperledgendary/fabric-devenv) virtual machine. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 22:43:46 +0000 UTC
    </div>
</div>

