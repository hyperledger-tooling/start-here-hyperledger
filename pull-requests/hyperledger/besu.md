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
                PR <a href="https://github.com/hyperledger/besu/pull/6254" class=".btn">#6254</a>
            </td>
            <td>
                <b>
                    [MINOR] fix log params for Failed to retrieve chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                We are logging this:
LOG.debug("Failed to retrieve chain head info. Disconnecting {}", peer, error);
Error is not printed 

Also noticed a similar issue in EthProtocolManager

before
```
2023-12-07 09:51:03.857	
2023-12-06 23:51:03.857+00:00 | EthScheduler-Timer-0 | DEBUG | ChainHeadTracker | Failed to retrieve chain head info. Disconnecting PeerId: 0xcbbaacaf47a005cb38... PeerReputation score: 99, timeouts: {3=1}, useless: 0, validated? true, disconnected? false, client: Geth/v1.13.2-stable-dc34fe82/linux-amd64/go1.21.1, [Connection with hashCode 2029564766 inboundInitiated? false initAt 1701906657037],...
```

after

`2023-12-07 13:19:53.174+10:00 | EthScheduler-Timer-0 | DEBUG | ChainHeadTracker | Failed to retrieve chain head info. Disconnecting 0x82b8a8b80c6c37caad... java.util.concurrent.TimeoutException: Timeout after 5000 MILLISECONDS`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 03:24:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6253" class=".btn">#6253</a>
            </td>
            <td>
                <b>
                    consensus/common migrate to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                redo of #6233 to fix DCO 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 02:19:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6252" class=".btn">#6252</a>
            </td>
            <td>
                <b>
                    increase parallelism usage back from mainnet AT
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 01:51:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6251" class=".btn">#6251</a>
            </td>
            <td>
                <b>
                    removed unnecessary use of static temp dir 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                ref #6248 removed further instances of static temp dir

Note some remaining ones, when changed, the tests failed - so I left them but added a comment. Some refactoring may be needed to get rid of those
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 01:05:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6249" class=".btn">#6249</a>
            </td>
            <td>
                <b>
                    migrate bft and some other ATs to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 22:28:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6248" class=".btn">#6248</a>
            </td>
            <td>
                <b>
                    Small fixes in main
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

fixes for issues discovered while debugging #6003 

static temp dir in PrivacyTest causes flaky test behavior.  fix by not using static temp dir:
<img width="1219" alt="Screenshot 2023-12-06 at 1 34 35 PM" src="https://github.com/hyperledger/besu/assets/1238512/3bf37877-dfb5-4f3a-a50b-51b933211d7c">

remove opinionated configs in debug docker image as they can cause difficult to discover failures/conflicts with existing network configs:
* explicit add of `*` to BESU_HOST_ALLOWLIST can cause ```Values '*' or 'all' can't be used with other hostnames``` if config has explict host configs (or even a duplicate `*` for hosts allow)
* explicit set of BESU_RPC_HTTP_API can cause ```Method not found``` for rpc namespaces added by config like for linea plugins, etc

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 21:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6247" class=".btn">#6247</a>
            </td>
            <td>
                <b>
                    fix: double calls to trace{Start,End}Transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This fixes double calls to trace{Start,End}Transaction.

## Fixed Issue(s)
Fixes #6246 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 11:33:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6244" class=".btn">#6244</a>
            </td>
            <td>
                <b>
                    Run ATs sequentially
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
This PR makes the ATs to run sequentially so we reduce the parallelism and get the build working again. This might result in a longer time for ATs to complete but right now Unit tests still take longer.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 05:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6243" class=".btn">#6243</a>
            </td>
            <td>
                <b>
                    [RPC] Use apiConfiguration to limit gasPrice in eth_getGasPrice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Use apiConfiguration to limit gasPrice in eth_getGasPrice

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 00:55:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6242" class=".btn">#6242</a>
            </td>
            <td>
                <b>
                    Code storage delete refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 23:09:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6241" class=".btn">#6241</a>
            </td>
            <td>
                <b>
                    Fix the annoying "Errors occurred while build effective model" during…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … builds

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Found a fix for the annoying build error 
```
Errors occurred while build effective model from [...]\.gradle\caches\modules-2\files-2.1\org.eclipse.platform\org.eclipse.swt\3.124.200\2013830105b55e3a9490b38034aef3c6f6c5862e\org.eclipse.swt-3.124.200.pom:
    'dependencies.dependency.artifactId' for org.eclipse.platform:org.eclipse.swt.${osgi.platform}:jar with value 'org.eclipse.swt.${osgi.platform}' does not match a valid id pattern. in org.eclipse.platform:org.eclipse.swt:3.124.200
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 18:55:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6239" class=".btn">#6239</a>
            </td>
            <td>
                <b>
                    update from main
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 16:57:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6237" class=".btn">#6237</a>
            </td>
            <td>
                <b>
                    Release 23.10.3
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 12:47:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6236" class=".btn">#6236</a>
            </td>
            <td>
                <b>
                    Update Gradle verification metadata
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

`./gradlew --no-daemon --write-verification-metadata sha256 spotlessCheck'

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 10:04:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6235" class=".btn">#6235</a>
            </td>
            <td>
                <b>
                    Pki - migrate to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #5560
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 06:37:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6234" class=".btn">#6234</a>
            </td>
            <td>
                <b>
                    crypto migrate to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #5568 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 05:31:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6232" class=".btn">#6232</a>
            </td>
            <td>
                <b>
                    Revert PR https://github.com/hyperledger/besu/pull/6187
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR reverts #6187. The PR causes syncing problems by not removing useless peers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 04:56:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6230" class=".btn">#6230</a>
            </td>
            <td>
                <b>
                    Deprecation warning if Forest pruning is enabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Forest pruning, option `pruning-enabled`, it is not maintained and this feature is superseded by Bonsai, no usage is reported also because to save disk space Bonsai is the solution and when using Forest usually the user want to keep all the history.
The proposal is to deprecated it now and remove it in few months, target 24.4 release

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 16:26:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6227" class=".btn">#6227</a>
            </td>
            <td>
                <b>
                    Release 23.10.3 rc1 in progress, uprev main.
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 19:42:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6226" class=".btn">#6226</a>
            </td>
            <td>
                <b>
                    Update OpenJ9 Docker image to latest version
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 18:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6225" class=".btn">#6225</a>
            </td>
            <td>
                <b>
                    Use `From` field in a `PING` packet when creating a peer table entry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR uses the `From` field of a `PING` packet when creating a local entry in the peer table, unless the `From` field is not available in which case it reverts to the existing behaviour of using the `UDP` source address.

Since (as far as I can tell) all `PING` packets include a `From` field (with `127.0.0.1` in the case where the user hasn't specified a custom value) the PR is coded to ignore a `From` field of `127.0.0.1` and use the UDP source address instead. The reality is that on a localhost system the UDP source will be `127.0.0.1` anyway but it provides a little extra protection from this change/fix causing issues on existing systems that might be working just fine using the UDP source address in peer's `enode` URL. The main aim of this fix is that if something **has** specified a custom value it is honoured by the `PING` recipient.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6224
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 15:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6222" class=".btn">#6222</a>
            </td>
            <td>
                <b>
                    [MINOR] move Pipeline stack trace to trace/debug level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log a message only at info
log stack trace at debug/trace depending on type of exception

fixes #5533 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 03:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6221" class=".btn">#6221</a>
            </td>
            <td>
                <b>
                    [MINOR] - Add plugin version summary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add plugin version summary
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 01:55:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6218" class=".btn">#6218</a>
            </td>
            <td>
                <b>
                    Allow `maxActiveConnections` for GraphQL and terminate requests based on actual connection status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

1. The option of `--graphql-http-max-active-connections` has been added to limit the numer of GraphQL requests served each time.
2. The GraphQL server has been relying on an `isAliveHandler` to terminate requests based on the timeout. However, this handler was only applied to `matchingLogs`, resulting in unterminated GraphQL executions in general even if the connection has timed out. Rather than relying on a future task, it is more appropriate to terminate requests based on the actual status of the connection. The `TimeoutHandler` should have handled the HTTP timeout while connections may also be terminated due to exceeding `maxActiveConnections`.

Docs change would be added in another PR in a later stage when code changes stabilise.

## Fixed Issue(s)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 15:40:58 +0000 UTC
    </div>
</div>

