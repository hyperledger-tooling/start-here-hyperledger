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
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    resolve #17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                try to resolve #17, Metrics and observability with [Prometheus and Grafana](./docs/prometheus.md)

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-31 13:17:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    Fix the api branch with latest apis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Updated api branch
* removed unwanted files

Signed-off-by: Ratnakar Asara <asara.ratnakar@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 17:10:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Bundle a localhost:5000 container registry for local CC development
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR bundles an insecure docker container registry at localhost:5000.  

During local build/edit/publish cycles for chaincode and gateway application development, the local registry can be used to publish docker images to k8s without uploading images to public / Internet-based registries. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 11:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    Adding changes for auto-cert renewal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: asararatnakar <asara.ratnakar@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 13:38:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/39" class=".btn">#39</a>
            </td>
            <td>
                <b>
                    Feature/prom - Configure prometheus on the sample network 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WORK IN PROGRESS - DO NOT MERGE 

This PR launches prometheus-operator on the sample network k8s cluster.  An ingress for prometheus and grafana are created at https://prometheus.localho.st and https://grafana.localho.st with a self-signed TLS certificate.

The test network includes a sample `ServiceMonitor` CRD for the org1-peer1.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 13:20:03 +0000 UTC
    </div>
</div>

