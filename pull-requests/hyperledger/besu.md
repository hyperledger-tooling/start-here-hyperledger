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
                PR <a href="https://github.com/hyperledger/besu/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    Try ignoring changelog
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2162" class=".btn">#2162</a>
            </td>
            <td>
                <b>
                    Change dev network chain ID to 1337
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change dev network chain ID to 1337

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
changed the dev network chain ID to 1337 instead of 2018 so that users can connect to Metamask "localhost 8545" network preset using default chainid settings

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2121 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 03:48:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2161" class=".btn">#2161</a>
            </td>
            <td>
                <b>
                    buildDocker depends on assemble only
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Run buildDocker in parallel with tests. publishDocker still happens after buildDocker AND all tests (but doesn't run on PRs)

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 03:00:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2160" class=".btn">#2160</a>
            </td>
            <td>
                <b>
                    ignore privateFor for tx estimation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Related to #2125, private tx estimation passes the `privateFor` field eg 
```
{"jsonrpc":"2.0","method":"eth_estimateGas","params":[{"from":"0x6402a0d7d3ed9db2163a234925e2bf82d45c7f99","gas":"0x47b760","value":"0x0","data":"0x608060405234801561001057600080fd5b5060405160208061011b8339810180604052602081101561003057600080fd5b505160005560d8806100436000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c806360fe47b11460375780636d4ce63c146053575b600080fd5b605160048036036020811015604b57600080fd5b5035606b565b005b605960a6565b60408051918252519081900360200190f35b60008190556040805182815290517f281b9a35503a0b511f50336e3e6b0d05a64fdadae7255e70f430feb2313c3c689181900360200190a150565b6000549056fea165627a7a7230582044f05a413bc5760ad1822322e6d8df2e38a8d78bb77512b03041026765408a1c0029","nonce":"0x0","privateFor":["FYmUrG0welC/cEm0buZsH9fjGeuETNZvZNeiROpy7XA="]}],"id":8}

```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 23:48:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2159" class=".btn">#2159</a>
            </td>
            <td>
                <b>
                    Update Reference Tests to 8.0.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 18:30:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2158" class=".btn">#2158</a>
            </td>
            <td>
                <b>
                    Remove Misleading Fast-Sync Logging
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
Users have been confused by this logging all the time. Probably best we remove those aspects that confuse them.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2156 
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 14:34:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2155" class=".btn">#2155</a>
            </td>
            <td>
                <b>
                    Refactor PermissioningConfiguration instantiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tidy up the way PermissioningConfiguration get propagated between `BesuCommand` and `BesuNode`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 09:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2154" class=".btn">#2154</a>
            </td>
            <td>
                <b>
                    Implement faucet for Aleut devnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Implements `debug_faucet` JSON RPC endpoint to enable users to request `ETH` on Aleut devnet. The endpoint takes one parameter which corresponds to the address of the recipient.

Adds 2 experimental flags:
-  `--Xfaucet-value`: Faucet value denominate in ETH (default: 5 ETH)
- `--Xfaucet-private-key`: Faucet account private key (default: first account in `dev.json` genesis)

## Usage

### Sample request
```
{
   "method":"debug_faucet",
   "id":1,
   "jsonrpc":"2.0",
   "params":[
      "0xC3298C6341f82468309302611e24D3003Bc79B46"
   ]
}
```

### Success response
```json
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": "0xb7d3183aff348d2d5994a978417129a4987d9f425295cc8e85b6563d2895a7bb"
}
```

### Unauthorized response
```json
{
    "jsonrpc": "2.0",
    "id": 1,
    "error": {
        "code": -40100,
        "message": "Unauthorized"
    }
}
```
## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Abdelhamid Bakhta <abdelhamid.bakhta@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 08:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2153" class=".btn">#2153</a>
            </td>
            <td>
                <b>
                    Update qbft reference test submodule with SPDX header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update qbft reference test submodule with SPDX header

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Usman Saleem <usman@usmans.info>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-19 02:13:11 +0000 UTC
    </div>
</div>

