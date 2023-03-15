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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1006" class=".btn">#1006</a>
            </td>
            <td>
                <b>
                    Update samples to use Fabric v2.5.0-beta2 by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update samples to use Fabric v2.5.0-beta2 by default.

Also remove pullFabricImages.sh since it is no longer used by anything.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 20:47:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1005" class=".btn">#1005</a>
            </td>
            <td>
                <b>
                    Fix Node HSM sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also:
- Tidy up README documentation.
- Add MacOS/Homebrew (Apple silicon) default SoftHSM library location to HSM scripts and sample applications to avoid the need to explicitly override the library location when running the sample.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 14:44:36 +0000 UTC
    </div>
</div>

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

