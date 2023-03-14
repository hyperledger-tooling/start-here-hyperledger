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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    Sample apps should exit code 1 upon failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure that all sample applications return exit code 1 upon failure so that github actions can report the failure.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 04:53:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    cfssl to generating certificates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new example to support pluggable CA in hyperledger fabric. Current examples in the `fabric-samples` provide two implementations for cert generation i.e `cryptogen` and `fabric-ca`. 

This PR will help the developers to understand more about bring your own identity. These changesets will allow developers to generate certificates using the [cfssl tool](https://github.com/cloudflare/cfssl), which is an opensource tool by cloudflare for cert management.

Generate certs using cfssl
```
./network.sh up -cfssl
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-12 09:20:47 +0000 UTC
    </div>
</div>

