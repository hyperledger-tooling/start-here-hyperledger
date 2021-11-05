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
                PR <a href="https://github.com/hyperledger/besu/pull/3008" class=".btn">#3008</a>
            </td>
            <td>
                <b>
                    When tls is on, use passthrough framer and passthrough handshaker to avoid double encryption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When tls is on, use passthrough framer and passthrough handshaker to avoid double encryption

Signed-off-by: Saravana Perumal Shanmugam <perusworld@linux.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 19:39:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2996" class=".btn">#2996</a>
            </td>
            <td>
                <b>
                    Improved QBFT logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                ## PR description
- Added some extra information on QBFT logs to help analysis

## Fixed Issue(s)
N/A

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 04:31:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2995" class=".btn">#2995</a>
            </td>
            <td>
                <b>
                    Qbft migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Spike of IBFT2 to QBFT migration. This is still a work in progress and is not intended to be merged as is.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 02:57:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2994" class=".btn">#2994</a>
            </td>
            <td>
                <b>
                    Added validate-config subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Fixes #2759 


I have tested this locally:

```
➜  besu git:(2837) ✗ besu validate-config --config-file ../besu-local-nodes/config/besu/besu1.conf
This toml config file is valid.%
➜  besu git:(2837) ✗ besu validate-config --config-file ../besu-local-nodes/config/besu/besu1.conf
picocli.CommandLine$ParameterException: Unknown option in TOML configuration file: xdata-path%
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 02:26:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2993" class=".btn">#2993</a>
            </td>
            <td>
                <b>
                    Log unused JSON params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2705. 

I have tested this locally. eg

```
{
    "jsonrpc": "2.0",
    "method": "eth_estimateGas",
    "params": [
        {
            "from": "0xFE3B557E8Fb62b89F4916B721be55cEb828dBd73",
            "to": "0xdd37f65db31c107f773e82a4f85c693058fef7a9",
            "nonce": 99,
            "value": "0x1"
        },
        "latest"
    ],
    "id": 1
}
```
gives me the expected result, with also this logged:
```
2021-11-04 11:35:17.486+10:00 | vert.x-worker-thread-14 | DEBUG | JsonCallParameter | unknown property - nonce with value - 99 and type - class java.lang.Integer caught during serialization
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 01:38:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2992" class=".btn">#2992</a>
            </td>
            <td>
                <b>
                    Update bls12-381 native library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The native library for bls12-381 is updated to the latest version to add support for M1 (ARM) processors.
 
## Fixed Issue(s)
Fixes #2668 

## Changelog

- [x ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 11:41:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2989" class=".btn">#2989</a>
            </td>
            <td>
                <b>
                    Add 21.10.0 release changes to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add 21.10.0 release changes from the release branch back to main
* update changelog to reflect the 21.10.0 release
* fix a bit of copypasta in retesteth chain params for the arrowGlacier definition

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 17:19:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2988" class=".btn">#2988</a>
            </td>
            <td>
                <b>
                    removes transitive deps on slf4j impl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Removes logback slf4j impl inherited from tuweni

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2800 
## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 13:46:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2986" class=".btn">#2986</a>
            </td>
            <td>
                <b>
                    [MINOR] Typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                typos

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 02:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    Add Daniel as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Add Daniel Lehrner as a contributor/maintainer.  

Daniel has contributed to hyperledger/besu significantly at ioBuilders  while working on adding secp256R1 support into besu, and he has recently joined the besu mainnet team at Consensys.

Daniel has already made significant contributions to [besu](https://github.com/hyperledger/besu/commits?author=daniel-iobuilders) and [besu-native](https://github.com/hyperledger/besu-native/pulls?q=is%3Apr+author%3Adaniel-iobuilders+), this PR proposes to add him as a maintainer.


https://github.com/hyperledger/besu/pull/2630
https://github.com/hyperledger/besu/pull/2321
https://github.com/hyperledger/besu/pull/2183
https://github.com/hyperledger/besu/pull/2163
https://github.com/hyperledger/besu/pull/2066
https://github.com/hyperledger/besu/pull/2036
https://github.com/hyperledger/besu/pull/2008
https://github.com/hyperledger/besu/pull/1933
https://github.com/hyperledger/besu-native/pull/48
https://github.com/hyperledger/besu-native/pull/45
https://github.com/hyperledger/besu-native/pull/39
https://github.com/hyperledger/besu-native/pull/38

## Vote
Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers [vote](https://github.com/hyperledger/besu/blob/master/MAINTAINERS.md#maintainers-approval-process).  

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 23:11:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2984" class=".btn">#2984</a>
            </td>
            <td>
                <b>
                    Release 21.10.0
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
        Created At 2021-11-01 22:00:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2983" class=".btn">#2983</a>
            </td>
            <td>
                <b>
                    Quarterly release branch update and cherry-pick
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Quarterly release for 21.10.0.  In addition to the cumulative release candidates (RC1, RC2, RC3, RC4):

* cherry-pick merge of arrow-glacier
* update CHANGELOG.md for quarterly release

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 20:38:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2980" class=".btn">#2980</a>
            </td>
            <td>
                <b>
                    [2950] Support websocket binary frames 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes https://github.com/hyperledger/besu/issues/2950

## Changelog

- Failing test for sending a binary frame to websocketservice
- Add support

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 05:41:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2979" class=".btn">#2979</a>
            </td>
            <td>
                <b>
                    Improve ValidatorContractController result validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add an extra check to ensure that a successful contract call with an empty result configures an error, as we never expect the validator contract to return an empty list of validators.

This is important because of the way that contract call works. It is possible to call an address that does not have a  contract deployed, and still get a successful call with an empty result.

## Fixed Issue(s)
fixes #2900

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-31 21:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2978" class=".btn">#2978</a>
            </td>
            <td>
                <b>
                    Feature/arrow glacier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Implement arrowGlacier hardfork EIP-4345.  

Upstream reference tests do not yet exist for arrowGlacier, but we can add them once they exist upstream, see #2977

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2943 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 20:09:49 +0000 UTC
    </div>
</div>

