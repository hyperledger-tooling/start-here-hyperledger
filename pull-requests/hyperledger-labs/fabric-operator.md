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
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    fix: use right operator-sdk version and support mac install
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```diff
- https://github.com/operator-framework/operator-sdk/releases/download/1.16.0/operator-sdk_linux_amd64
+ https://github.com/operator-framework/operator-sdk/releases/download/v1.16.0/operator-sdk_linux_amd64
```

please see https://github.com/operator-framework/operator-sdk/releases/tag/v1.16.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 09:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Use PodSecurity Admission controller for k8s versions v1.25.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger-labs/fabric-operator/issues/50
Thank you @celder628 for the notes.

Signed-off-by: asararatnakar <asara.ratnakar@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-11 12:43:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    chore: remove todo in unit-tests workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                uncomment push and gosec
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 06:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    chore: remove same code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the line87-89 and line 91-93 is same, but twice:

https://github.com/hyperledger-labs/fabric-operator/blob/db38e856fda7798650de925addadbc75305adc39/integration/orderer/orderer_suite_test.go#L85-L97

And line 205 and 206 is same but twice:

https://github.com/hyperledger-labs/fabric-operator/blob/db38e856fda7798650de925addadbc75305adc39/pkg/offering/k8s/orderer/node.go#L203-L210
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 06:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    chore: push image workflow should limit repository
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The idea of automatically building the image and pushing it to the `ghcr.io` repository after the pull request merge is great. 

Just one small restriction: only run the push job on the main repository: `hyperledger-labs/fabric-operator`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 03:02:55 +0000 UTC
    </div>
</div>

