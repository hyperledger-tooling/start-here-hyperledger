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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2181" class=".btn">#2181</a>
            </td>
            <td>
                <b>
                    add support for 1559 in retesteth besu command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
* add support for 1559 in test_setChainParams 
* add a "1559 at genesis" provision

This pr kicks the can down the road for 2 things: 
* hardfork naming
* 1559 baseFee as a part of genesis json configuration

the first is NBD, but we might want to incorporate baseFee in genesis config at some point.  Probably once we move 1559 out of 'experimental' status.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2180

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 22:03:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2179" class=".btn">#2179</a>
            </td>
            <td>
                <b>
                    Add downlink for 21.1.5 release
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

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 17:54:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2178" class=".btn">#2178</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.1.6-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 17:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2176" class=".btn">#2176</a>
            </td>
            <td>
                <b>
                    Release 21.1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 16:52:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2172" class=".btn">#2172</a>
            </td>
            <td>
                <b>
                    check that doesn't break during release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `dev` isn't present in the version string during a release. `besu` is, however.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 16:27:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2169" class=".btn">#2169</a>
            </td>
            <td>
                <b>
                    Prepare changelog for release 21.1.5
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

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 15:19:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2166" class=".btn">#2166</a>
            </td>
            <td>
                <b>
                    Tessera Orion-mode privacy ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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
        Created At 2021-04-21 04:23:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2165" class=".btn">#2165</a>
            </td>
            <td>
                <b>
                    Remove docker-ro creds from circle ci pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Change to docker creds handling so that CI can run on external contributors' PRs

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
n/a

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 14:58:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2164" class=".btn">#2164</a>
            </td>
            <td>
                <b>
                    Bonsai trie : fix consensus issue on ropsten
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

Fix an invalid originalValue for a specific storage slot :

in the same block we are doing
1 ) create a contract
2) change the value of a slot
3) change a second time the value of the same slot. the original is empty while it should be the previous value of the step 2

Why because when we create a contract we clear the storage so the method return 0x 

https://github.com/hyperledger/besu/blob/e13dd77c8d3a4ad6b003d2c71526a39818195ea8/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/bonsai/BonsaiWorldStateUpdater.java#L314

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 10:13:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2163" class=".btn">#2163</a>
            </td>
            <td>
                <b>
                    Fix: Native libraries of secp256k1 and alt bn 128 can be disabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR fixes the ability to disable the native library implementations for secp256k1 and altBn128 via the command line. I added a log message in case of using the Java implementation, to make it clear to the user which implementation is used in both cases.

## Fixed Issue(s)
fixes #2150 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 08:44:41 +0000 UTC
    </div>
</div>

