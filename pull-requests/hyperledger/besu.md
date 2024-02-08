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
                PR <a href="https://github.com/hyperledger/besu/pull/6539" class=".btn">#6539</a>
            </td>
            <td>
                <b>
                    Fix checkLicense gradle task
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
I'm getting a gradle build failure due the "checkLicenses" task.  This looks like a misspelling:
```
% ./gradlew dev -x test

FAILURE: Build failed with an exception.

* What went wrong:
Task 'checkLicenses' not found in root project 'besu' and its subprojects. Some candidates are: 'checkLicense'.
```

Fix this by using the existin "checkLicense" task.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 00:04:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6537" class=".btn">#6537</a>
            </td>
            <td>
                <b>
                    Github Actions Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Uses `pull_request_target` to make sure action definitions only come from `main` or `release-*`. This also allows them to escalate privs.
- All priv escalations moved as narrowly as possible. Typically this is only required to upload test results.
- All actions pinned to specific SHA versions. When updated, repository settings will need to be adjusted to allow it.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 17:39:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6536" class=".btn">#6536</a>
            </td>
            <td>
                <b>
                    Default storage format now Bonsai 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Builds on #6530 
Refs #5391 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 02:26:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6534" class=".btn">#6534</a>
            </td>
            <td>
                <b>
                    [minor] Improve message when existing database is different from the configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ux</span>
            </td>
            <td>
                ## PR description

Improve message error when existing database with a different version is detected

`Mismatch: DB at '/path' is FOREST (Version 1) but config expects BONSAI (Version 2). Please check your config.`

see: #5926
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 13:10:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6533" class=".btn">#6533</a>
            </td>
            <td>
                <b>
                    Add missing javadoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add missed javadoc for `ClassicEVM` from #6524
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 12:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6530" class=".btn">#6530</a>
            </td>
            <td>
                <b>
                    Make SNAP the default sync mode for named networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refs #5391
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 09:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6528" class=".btn">#6528</a>
            </td>
            <td>
                <b>
                    error if snap or checkpoint sync specified with privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                we enforce that you can't specify FAST sync if privacy is enabled - do the same check for SNAP and CHECKPOINT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 06:23:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6526" class=".btn">#6526</a>
            </td>
            <td>
                <b>
                    Acceptance Tests - only run non-privacy ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                exclude privacy tests since they are currently flaky (they are run on a separate nightly cadence)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 01:33:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6525" class=".btn">#6525</a>
            </td>
            <td>
                <b>
                    Better tracing alignment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Update tracing and evm tool
* Intrinsic gas is optional in EVMTool
* For call series, also charge the gas given to the next call level

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #6523
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 00:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6524" class=".btn">#6524</a>
            </td>
            <td>
                <b>
                    Add ETC Spiral EVM configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
During the last ETC network upgrade, Besu nodes got stalled because, inadvertently, [EIP-4399](https://eips.ethereum.org/EIPS/eip-4399) was _included_ instead of _omitted_.

For the future, we'll also test omissions to the protocol and not only additions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-05 05:14:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6522" class=".btn">#6522</a>
            </td>
            <td>
                <b>
                    increase timeout for websocket pub/sub tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">flake</span>
            </td>
            <td>
                Increase timeout for websocket ATs since a few of them are flaky eg https://app.circleci.com/pipelines/github/hyperledger/besu/27037/workflows/036ea38e-b0b0-4e2e-8d9c-a280f53134e3/jobs/179105/tests#failed-test-0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-04 23:19:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6521" class=".btn">#6521</a>
            </td>
            <td>
                <b>
                    tx-pool allow/reject list
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
This PR adds the following flags to configure allow/reject list of sender addresses 

- `--tx-pool-allow-list=<comma-seprated-list-of-addresses>` - Local/Remote transactions submitted from these addresses are only allowed to be added in the pool, while transactions from other sender addresses are reject with reason `Sender account not authorized to send transactions`
- `--tx-pool-reject-list=<comma-seprated-list-of-addresses>` - Local/Remote transactions submitted from these addresses are rejected before being added to the pool with reason `Sender account not authorized to send transactions`, while transactions from other sender addresses are allowed.
- Both these flags are not allowed together, only one can be set at a time. 

**Sample Besu Log**
Setting the following config for test addresses and sending test transaction from these accounts 
`tx-pool-reject-list=["0x8C7d8409bDBA3322A65825bbe3f75ac71b9de3cf,0xe547BAa69dB4fCFd6225f428De424888dB566a41"]` for test 
```
2024-02-04 21:47:20.559+00:00 | vert.x-worker-thread-1 | TRACE | AbstractJsonRpcExecutor | {"jsonrpc":"2.0","id":83,"method":"eth_sendRawTransaction","params":["0xf8868080830f4240944fca308301a110a0118448c644654efeecf9a91180a460fe47b10000000000000000000000000000000000000000000000000000000000003039820ff1a0777743d184749836701b2bdc63c35f89523ae804291696cf6d5778e24aa1240aa07ff93a28da5138dd50277ec7b3249b03736eaa8cc99c035503131eccb6e5b04c"]}
2024-02-04 21:47:20.559+00:00 | vert.x-worker-thread-1 | DEBUG | JsonRpcExecutor | JSON-RPC request -> eth_sendRawTransaction ["0xf8868080830f4240944fca308301a110a0118448c644654efeecf9a91180a460fe47b10000000000000000000000000000000000000000000000000000000000003039820ff1a0777743d184749836701b2bdc63c35f89523ae804291696cf6d5778e24aa1240aa07ff93a28da5138dd50277ec7b3249b03736eaa8cc99c035503131eccb6e5b04c"]
2024-02-04 21:47:20.560+00:00 | vert.x-worker-thread-1 | TRACE | EthSendRawTransaction | Received local transaction MessageCall{type=FRONTIER, nonce=0, gasPrice=0 wei, gasLimit=1000000, to=0x4fca308301a110a0118448c644654efeecf9a911, value=0x0000000000000000000000000000000000000000000000000000000000000000, sig=Signature{r=54035951847700603082610381881786735130294417072039064688183051346590583301130, s=57884078091882121988970232755018579959487602981021234593703990990705896304716, recId=0}, chainId=2023, payload=0x60fe47b10000000000000000000000000000000000000000000000000000000000003039}
2024-02-04 21:47:20.560+00:00 | vert.x-worker-thread-1 | TRACE | TransactionPool | Discarded transaction from unauthorized sender 0x8c7d8409bdba3322a65825bbe3f75ac71b9de3cf
2024-02-04 21:47:20.560+00:00 | vert.x-worker-thread-1 | TRACE | AbstractJsonRpcExecutor | {"jsonrpc":"2.0","id":83,"error":{"code":-32007,"message":"Sender account not authorized to send transactions"}}
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes Issue https://github.com/hyperledger/besu/issues/5243
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-04 22:23:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6520" class=".btn">#6520</a>
            </td>
            <td>
                <b>
                    [MINOR] Fix typo on github action checklist 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 06:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6519" class=".btn">#6519</a>
            </td>
            <td>
                <b>
                    [MINOR] Move log before where the subcommand hangs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Indicate pruning has begun before the subcommand starts processing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 05:52:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6518" class=".btn">#6518</a>
            </td>
            <td>
                <b>
                    Change contract creation halt reason when account already exists
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
Change the execution halt reason from INSUFFICIENT_GAS to ILLEGAL_STATE_CHANGE to reflect the real reason behind this case which is a possible contract creation collision with a already existing a account at that address.

Note that some of the trace ATs had to be adjusted after this change, possibly because the frame where we fail execution was getting included into the trace result as we don't ignore frames that halted due to INSUFFICIENT_GAS https://github.com/hyperledger/besu/blob/2a30dfba1a03ad1c2b9d42857615984c439f4970/ethereum/api/src/main/java/org/hyperledger/besu/ethereum/api/jsonrpc/internal/results/tracing/vm/VmTraceGenerator.java#L110
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 04:50:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6517" class=".btn">#6517</a>
            </td>
            <td>
                <b>
                    [minor] Add staker profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Add staker profile

Use:
`besu --profile=staker`

More: [#6409](https://github.com/hyperledger/besu/issues/6409)

## Fixed Issue(s)
fixes [#6325](https://github.com/hyperledger/besu/issues/6325)
see: [#6323](https://github.com/hyperledger/besu/issues/6323)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 04:04:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6516" class=".btn">#6516</a>
            </td>
            <td>
                <b>
                    Close Sockets after testing for availablity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Close the Sockets after checking for their availability.
Also makes the code more readable by checking for unavailability not availability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 02:12:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6513" class=".btn">#6513</a>
            </td>
            <td>
                <b>
                    [MINOR] Detect DB version mismatch on Startup and gracefully exit #6511
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Detect DB version mismatch on Startup and gracefully exit

Message:

`Mismatch detected: Database at ./database is version '1', but configuration expects version '2'.
`
## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/5926
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 05:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6512" class=".btn">#6512</a>
            </td>
            <td>
                <b>
                    [Refactor] Move api options to its own class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move api options options to its own class

## Fixed Issue(s)
see https://github.com/hyperledger/besu/issues/6428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 04:06:12 +0000 UTC
    </div>
</div>

