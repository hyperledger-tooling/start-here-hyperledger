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
                PR <a href="https://github.com/hyperledger/besu/pull/6267" class=".btn">#6267</a>
            </td>
            <td>
                <b>
                    ETC mainnet 'Spiral' activation block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR sets ETC Mainnet activation block as defined in [ECIP-1109](https://ecips.ethereumclassic.org/ECIPs/ecip-1109) to `19_250_000`. This change was already merged in core-geth in https://github.com/etclabscore/core-geth/pull/595
I also set the DNS discovery tree to what's in [core-geth#bootnodes_classic.go](https://github.com/etclabscore/core-geth/blob/v1.12.17/params/bootnodes_classic.go#L28)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 20:12:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6260" class=".btn">#6260</a>
            </td>
            <td>
                <b>
                    Non bft group ats junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                this is #6249 without clique/bft ATs
fixes #6265
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 23:18:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6259" class=".btn">#6259</a>
            </td>
            <td>
                <b>
                    Fix and test that the BlockAwareOperationTracer methods are invoked the correct number of times
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

@delehef please double check the removal of redundant calls to `traceEndBlock`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

tests & fixes #6246

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 12:51:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6258" class=".btn">#6258</a>
            </td>
            <td>
                <b>
                    migrate permissioning ATs to junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #6262 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 08:29:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6256" class=".btn">#6256</a>
            </td>
            <td>
                <b>
                    plugin and jsonrpc ATs to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #6264 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 06:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6255" class=".btn">#6255</a>
            </td>
            <td>
                <b>
                    add extra gradle task dependency to silence warning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                Seems redundant but it fixes this warning

```
Execution optimizations have been disabled for task ':acceptance-tests:tests:processTestResources' to ensure correctness due to the following reasons:
  - Gradle detected a problem with the following location: '/Users/sallymacfarlane/workspace/b2/acceptance-tests/test-plugins/build/libs'. Reason: Task ':acceptance-tests:tests:processTestResources' uses this output of task ':acceptance-tests:test-plugins:jar' without declaring an explicit or implicit dependency. This can lead to incorrect results being produced, depending on what order the tasks are executed. Please refer to https://docs.gradle.org/7.6/userguide/validation_problems.html#implicit_dependency for more details about this problem.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 06:37:33 +0000 UTC
    </div>
</div>

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
This PR increases the parallelism back to 4 to try and get the mainnet AT's back to a good state.
## Fixed Issue(s)
Fixes #6250 
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
                    migrate bft and clique ATs to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #6261
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

