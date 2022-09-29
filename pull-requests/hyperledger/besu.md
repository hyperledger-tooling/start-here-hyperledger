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
                PR <a href="https://github.com/hyperledger/besu/pull/4457" class=".btn">#4457</a>
            </td>
            <td>
                <b>
                    Avoid sending added blocks to transaction pool during initial sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

22.7.4 has a regression on initial sync time, due to the fact that imported blocked are sent to the transaction pool even if it is empty until the initial   sync is done, and in 22.7.4 for every transaction in the block getSender is called and that consume a lot of CPU, to fix in PR#4457 I just make the tx pool subscribe to block added events only when the initial sync is done

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 13:40:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4456" class=".btn">#4456</a>
            </td>
            <td>
                <b>
                    WIP - Migrate deprecated features in picocli to v4.0
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
This PR migrates deprecated features in picocli to the recommended for 4.0
- Replaces parseWithHandles by the execute API
- Replaces deprecated interfaces by their equivalent in picocli 4.0

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #2701 
## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 05:47:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4455" class=".btn">#4455</a>
            </td>
            <td>
                <b>
                    Keep the best block built until now instead of the last one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

If the consensus layer client, send more than once the same forkchoice update with payload attributes, we build more blocks with the same payload id, but the current implementation just keep the latest one built, no matter if it is better or not than the existing ones.
This PR improve that, comparing the blocks with the same payload id, and keeping the best according to the amount of gas used, this could be improved in a next iteration, comparing the actual fee reward of the block.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 16:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4451" class=".btn">#4451</a>
            </td>
            <td>
                <b>
                    Prints configuration overview
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

Prints an overview of configuration and system information at startup. This is considered a first version and mainly intended to help debug issues that users on Ethereum Mainnet experience.

![Screenshot from 2022-09-28 09-12-20](https://user-images.githubusercontent.com/6727189/192712632-412c5ebf-e23f-49e0-a731-f08581c39b7c.png)

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 19:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4449" class=".btn">#4449</a>
            </td>
            <td>
                <b>
                    Access fields/methods more directly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

* `Mockito#any` is more directly accessible via `ArgumentMatchers#any`
* `DefaultFunctionReturnDecode#decode` is more directly accessible via `FunctionReturnDecoder#decode`

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 19:39:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4448" class=".btn">#4448</a>
            </td>
            <td>
                <b>
                    Fix a few output string issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

* Fix some minor spacing issues.
* Fix a string concatenation & numeric addition order of operations issue.

The following example will result in a block number of 11 being printed, instead of 2.

```java
public class Main
{
    public static void main(String[] args) {
        long blockNumber = 1;
        System.out.println("Invalid block number: " + blockNumber + 1);
    }
}
```

```
Invalid block number: 11
```

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 19:18:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4447" class=".btn">#4447</a>
            </td>
            <td>
                <b>
                    Update Security Policy contact info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

At the request of the EF, a besu-only security list was created, and is the first listed email.  The out-of-date Jira location is also removed.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 18:57:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4445" class=".btn">#4445</a>
            </td>
            <td>
                <b>
                    Update everything_config.toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: inDane <inDane@users.noreply.github.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Additional to #4438 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 11:36:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4444" class=".btn">#4444</a>
            </td>
            <td>
                <b>
                    updated version and CHANGELOG for next dev cycle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 17:08:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4442" class=".btn">#4442</a>
            </td>
            <td>
                <b>
                    adding new release version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## 22.7.4


### Bug Fixes
- Remove records that track transactions by sender when they are empty to same memory in the transaction pool [#4415](https://github.com/hyperledger/besu/pull/4415)
- Add Toml configuration file support for _--Xplugin-rocksdb-high-spec-enabled_ flag

Signed-off-by: Justin Florentine <justin+github@florentine.us>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 15:58:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4438" class=".btn">#4438</a>
            </td>
            <td>
                <b>
                    Add config file support for high spec flag
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
With PR #4423, the flag --Xplugin-rocksdb-high-spec-enabled doesn't work with Toml configuration files. This PR fix this issue.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-25 15:02:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4433" class=".btn">#4433</a>
            </td>
            <td>
                <b>
                    post-22.7.3 changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

post-release changelog update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 17:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4432" class=".btn">#4432</a>
            </td>
            <td>
                <b>
                    these don't need to be at info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 17:30:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4431" class=".btn">#4431</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.7.4-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.7.4-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 16:57:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4430" class=".btn">#4430</a>
            </td>
            <td>
                <b>
                    Release 22.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.7.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 16:25:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4427" class=".btn">#4427</a>
            </td>
            <td>
                <b>
                    add engine_preparePayload_debug endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Draft PR to enable debugging block proposals by re-adding an updated version of the deprecated 
`engine_preparePayload` endpoint

*be sure to use the current or a recent parent blockhash or you will DoS bonsai db*
example usage:
```
curl --location --request POST 'http://localhost:8551' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE2NTkwNDEzMzZ9.4PDdSaG9hFOFR4Th7rEgaKKECsXfz6IPckFRcfSP13o' \
--data-raw '{
    "jsonrpc":"2.0",
    "method":"engine_preparePayload_debug",
    "params":
    [
        {
            "parentHash": "0xd4e56740f876aef8c010b86a40d5f56745a118d0906a34e69aec8c0db1cb8fa3",
            "feeRecipient": "0x0000000000000000000000000000000000000000",
            "timestamp": "0x0",
            "prevRandao": "0x0"
        }
    ],
    "id":1
}'
```



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 21:34:42 +0000 UTC
    </div>
</div>

