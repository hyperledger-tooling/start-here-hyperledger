---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2199" class=".btn">#2199</a>
            </td>
            <td>
                <b>
                    Add check to avoid useless modification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 13:51:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2197" class=".btn">#2197</a>
            </td>
            <td>
                <b>
                    fix selection of receive RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are two RPC in Tessera for GET "/transaction/{hash}". This makes sure we are using the right one.

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 01:05:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2196" class=".btn">#2196</a>
            </td>
            <td>
                <b>
                    Removed container test build step.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Removing the container test build step until the privacy issue is resolved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 21:21:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2193" class=".btn">#2193</a>
            </td>
            <td>
                <b>
                    Address 1559 config assumption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                address assumption that if 1559 is enabled there is a london fork block config
fixes #2192

Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 23:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    Ignoring changelog modification on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

During releases we can waste time waiting for the pipeline while we only change the CHANGELOG. This PR will not run the tests if we only modify the CHANGELOG

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 13:45:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2184" class=".btn">#2184</a>
            </td>
            <td>
                <b>
                    fix GoQuorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The /receive RPC method that was used by Besu to retrieve private transactions in qoQuorum privacy mode from Tessera has been removed. This PR changes Besu to use the same RPC that is used by GoQuorum.

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 03:13:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2183" class=".btn">#2183</a>
            </td>
            <td>
                <b>
                    Add SECP256R1 support to CLI sub command generate-blockchain-config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Support for secp256r1 is added to the CLI sub command `generate-blockchain-config`. The command checks if the genesis property of the configuration file has a field `ecCurve`. This field is used to select the alternative signature algorithm secp256r1. If secp256r1 is indeed set, the public keys in extraData are generated using this signature algorithm. In any other case the default signature algorithm is used.
If the public keys are already provided in the blockchain property of the configuration file, it is verified if those keys are valid for the selected signature algorithm. This avoids that a user error could generate a genesis file with invalid keys.

## Fixed Issue(s)
Fixes #2182 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 20:53:26 +0000 UTC
    </div>
</div>

