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
                PR <a href="https://github.com/hyperledger/besu/pull/3022" class=".btn">#3022</a>
            </td>
            <td>
                <b>
                    Maintainer: add Taccat Isid 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I propose to add @taccatisid as a Besu project maintainer.

@taccatisid has contributed with many high quality commits:

Here are their past contributions on Besu project
- https://github.com/hyperledger/besu/pull/2644
- https://github.com/hyperledger/besu/pull/2674
- https://github.com/hyperledger/besu/pull/2717
- https://github.com/hyperledger/besu/pull/2805
- https://github.com/hyperledger/besu/pull/2956

<!-- for non-code contributors -->
@taccatisid also contributed with many high quality actions:

Quality code reviews eg 
- https://github.com/hyperledger/besu/pull/2994
- https://github.com/hyperledger/besu/pull/2971

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers [vote](https://github.com/hyperledger/besu/blob/main/MAINTAINERS.md#maintainers-approval-process).

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 20:38:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3021" class=".btn">#3021</a>
            </td>
            <td>
                <b>
                    Fix a double execution of the same method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

description in https://github.com/hyperledger/besu/issues/3020

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3020

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 18:09:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3018" class=".btn">#3018</a>
            </td>
            <td>
                <b>
                    JsonUtil.normalizeKeys should handle ArrayNodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Updated JsonUtils to handle ArrayNode. This is important now that we have bft transitions that are specified in an array in the genesis file.

## Fixed Issue(s)
fixes #2856

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 05:15:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3017" class=".btn">#3017</a>
            </td>
            <td>
                <b>
                    [2981] Multi algorithm support for JWT
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
Fixes #2981 

## Changelog

Add support for additional JWT auth algorithms and associated tests

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 04:39:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3016" class=".btn">#3016</a>
            </td>
            <td>
                <b>
                    separate step for sonar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Separate SonarQube into its own step since it uses a restricted context

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 02:24:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3014" class=".btn">#3014</a>
            </td>
            <td>
                <b>
                    More BFT tracing log messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Add a trace log message when `BftProtocolManager` receives a subprotocol message. This is the entry-point for BFT related logic in response to the message.

## Fixed Issue(s)
N/A

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 01:43:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3008" class=".btn">#3008</a>
            </td>
            <td>
                <b>
                    When tls is on, use plain framer and handshaker to avoid double encryption
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

