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
                PR <a href="https://github.com/hyperledger/besu/pull/3837" class=".btn">#3837</a>
            </td>
            <td>
                <b>
                    Fcu verify payload attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adds payload attributes checks to EngineForkchoiceUpdated and returns INVALID_PAYLOAD_ATTRIBUTES error if any of them should be invalid.

## Fixed Issue(s)
"fixes #3836 "

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-15 22:19:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3835" class=".btn">#3835</a>
            </td>
            <td>
                <b>
                    Ref tests 10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description
Upgrade reference Tests to 10.3

10.3 revision of reference tests has notable changes

* Nonce can be up to 2^64-1, with some opcode and validity interactions 
  specced in eip-2681
* Wei fields can be up to 2^256, tests check for rollover
* VM Tests were removed
* Legacy Tests were removed

Includes changes from PR #3747 
 
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
        Created At 2022-05-14 07:28:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3834" class=".btn">#3834</a>
            </td>
            <td>
                <b>
                    3619 unify rpc ports
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

- Introduces new JsonRPCService that handles both http and websockets
- Removes websocket specific configs
- renames WebSocketRequestHandler to WebSocketMessageHandler to be more in line with websocket semantics.

## Fixed Issue(s)

fixes #3619 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 16:07:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3832" class=".btn">#3832</a>
            </td>
            <td>
                <b>
                    Reduce EVM library dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce the runtime dependencies of the EVM module by moving a
class used by a single class out of util to the owned module (QosTimer)
and them removing un-used dependencies from EVM and dependant modules.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 02:33:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3831" class=".btn">#3831</a>
            </td>
            <td>
                <b>
                    Added Metrics for number of open RPC connections[#3781]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added Metrics for number of open RPC connections - besu_rpc_active_http_connection_count, besu_rpc_active_ws_connection_count

Signed-off-by: Sharad Gulati sharad.develop@gmail.com

## Fixed Issue(s)
fixes #3781 

## Documentation

- [ x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
Documentation might need to be updated due to additional metrics

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 01:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3830" class=".btn">#3830</a>
            </td>
            <td>
                <b>
                    quorum ATs can run on medium executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Change quorum ATs (nightly) from XL to medium executor. 

The job ran successfully on medium executor https://app.circleci.com/pipelines/github/hyperledger/besu/14864/workflows/e1c2b5d0-44b1-45aa-a5c6-f46eeca7f4bc/jobs/85796

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 01:41:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3828" class=".btn">#3828</a>
            </td>
            <td>
                <b>
                    Return Invalid forkchoice state if fcU contains invalid finalizedBlockHash or safeBlockHash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

When engine_forkchoiceUpdatedV1 is called we need to check that the blocks of finalizedBlockHash and safeBlockHash belong to the chain defined by headBlockHash

## Fixed Issue(s)
fixes #3827 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 11:43:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3826" class=".btn">#3826</a>
            </td>
            <td>
                <b>
                    Sync Downloaders  now implement common interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a step towards unifying sync downloaders under a common interface with start/stop methods

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 09:03:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3825" class=".btn">#3825</a>
            </td>
            <td>
                <b>
                    Performance test : add the name of the Pipeline's step in Tracing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This test will help to identify the name of the Pipeline's step during execution. 
This will help to identify which step is waiting for others to complete.
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
        Created At 2022-05-12 08:53:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3823" class=".btn">#3823</a>
            </td>
            <td>
                <b>
                    warning for clique consensus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Since we don't recommend clique for production
* add a warning if starting Besu with clique consensus
* add a CLI option `--Xclique-enabled` which must be true for Besu to start with clique 

With default=true, not breaking change - but we probably want to do that in the future. 
With default=false, this will be a breaking change - anyone using clique will need to add this CLI option

```
➜  besu-local-nodes git:(multi-tenancy) ✗ besu --config-file=config/besu/besu1-quorum.conf  --Xclique-enabled=false
Setting logging level to INFO
Clique consensus recommended for dev/test networks only. To force, use --Xclique-enabled

To display full help:
besu [COMMAND] --help
➜  besu-local-nodes git:(multi-tenancy) ✗ besu --config-file=config/besu/besu1-quorum.conf
Setting logging level to INFO
2022-05-12 15:41:26.450+10:00 | main | INFO  | Besu | Using LibEthPairings native alt bn128
2022-05-12 15:41:26.452+10:00 | main | INFO  | Besu | Using the native implementation of the signature algorithm
2022-05-12 15:41:26.456+10:00 | main | INFO  | Besu | Starting Besu version: besu/v22.4.1-dev-46252afe/osx-x86_64/openjdk-java-11
2022-05-12 15:41:27.098+10:00 | main | WARN  | Besu | Discovery disabled: bootnodes will be ignored.
2022-05-12 15:41:27.102+10:00 | main | WARN  | Besu | Permissions are disabled. Cannot enable PERM APIs when not using Permissions.
2022-05-12 15:41:27.102+10:00 | main | INFO  | Besu | Static Nodes file = /Users/sallymacfarlane/workspace/besu-local-nodes/workdir/besu1/data/static-nodes.json
2022-05-12 15:41:27.104+10:00 | main | INFO  | StaticNodesParser | StaticNodes file /Users/sallymacfarlane/workspace/besu-local-nodes/workdir/besu1/data/static-nodes.json does not exist, no static connections will be created.
2022-05-12 15:41:27.105+10:00 | main | INFO  | Besu | Connecting to 0 static nodes.
2022-05-12 15:41:27.107+10:00 | main | INFO  | Besu | Security Module: localfile
2022-05-12 15:41:27.127+10:00 | main | INFO  | DatabaseMetadata | Lookup database metadata file in data directory: /Users/sallymacfarlane/workspace/besu-local-nodes/workdir/besu1/data
2022-05-12 15:41:27.184+10:00 | main | INFO  | RocksDBKeyValueStorageFactory | Existing database detected at /Users/sallymacfarlane/workspace/besu-local-nodes/workdir/besu1/data. Version 1
2022-05-12 15:41:28.857+10:00 | main | WARN  | Besu | Discovery disabled: bootnodes will be ignored.
2022-05-12 15:41:28.863+10:00 | main | WARN  | BesuController |
***************
We recommend Clique for use in development and test networks (Goerli and Rinkeby) only. For production, please use QBFT.
***************
2022-05-12 15:41:28.879+10:00 | main | INFO  | KeyPairUtil | Loaded public key 0xfcbe9f83218487b3c0b50878193880e6c25cfd86708c0a0bf0ca91f0ce633746a892fe240afa5b9a880b8bca48e8a22704ef937fdda2d7cc63e4d41ed1b417ae from /Users/sallymacfarlane/workspace/besu-local-nodes/workdir/besu1/keys/besu1.priv
```

## Documentation

- [] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 05:47:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3822" class=".btn">#3822</a>
            </td>
            <td>
                <b>
                    Group headings for P2P discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                Add P2P Discovery Options to group related options
* Reworking of #3692 - thanks to @sandrawangyx 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 02:03:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3821" class=".btn">#3821</a>
            </td>
            <td>
                <b>
                    [MINOR] one more test for allowlist / DNS scenario
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added one more test for the permissioning / allowlist / DNS host resolution issue see #3804 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 00:25:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3820" class=".btn">#3820</a>
            </td>
            <td>
                <b>
                    Circle-ci branch filter for dockerManifest 
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
fix branch filter for dockerManifest task in circleci to reference `main` rather than `master`

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
        Created At 2022-05-11 20:26:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3818" class=".btn">#3818</a>
            </td>
            <td>
                <b>
                    fix and reinstate the ignored dns/permissioning/allowlist test 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Test was failing because enode containing IP was being resolved via DNS to a hostname, but assertion was still checking for IP. 

Added tests for allowlist behaviour with DNS enabled:
* add enode with IP and then same enode with hostname throws exception
* add enode with hostname should "just work" 
* add enode with IP will resolve to DNS hostname. So check with this behaviour by creating the enodeUrl with DNS config

debug logs from CI
```
03:56:50.876 | Test worker | INFO  | AllowlistWithDnsEnodePersistorAcceptanceTest | enode 2 string enode://5f8a80d14311c39f35f516fa664deaaaa13e85b2f7493f37f6144d86991ec012937307647bd3b9a82abe2974e1407241d54947bbb39763a4cac9f77166ad92a0@192.168.0.10:1234
03:56:50.916 | Test worker | INFO  | AllowlistWithDnsEnodePersistorAcceptanceTest | enodeURL 2 with DNS enabled but NOT dns update enode://5f8a80d14311c39f35f516fa664deaaaa13e85b2f7493f37f6144d86991ec012937307647bd3b9a82abe2974e1407241d54947bbb39763a4cac9f77166ad92a0@192.168.0.10:1234
03:56:50.934 | Test worker | INFO  | AllowlistWithDnsEnodePersistorAcceptanceTest | enodeURL 2 with DNS enabled AND dns update enode://5f8a80d14311c39f35f516fa664deaaaa13e85b2f7493f37f6144d86991ec012937307647bd3b9a82abe2974e1407241d54947bbb39763a4cac9f77166ad92a0@ip-192-168-0-10.ec2.internal:1234
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
        Created At 2022-05-11 09:27:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3816" class=".btn">#3816</a>
            </td>
            <td>
                <b>
                    Fix for multi-arch docker develop and latest tags 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

In the multi-arch docker build pr #2954, the manifest step is not correctly creating the `develop` and `latest` multi-arch tags.  This pr fixes the tag creation in the manifestDocker step

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
        Created At 2022-05-11 04:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3815" class=".btn">#3815</a>
            </td>
            <td>
                <b>
                    Migrate integrationTests to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As an effort to modularize Junit5 migration, this PR only migrates tests ran from the `integrationTest` task.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 00:46:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3814" class=".btn">#3814</a>
            </td>
            <td>
                <b>
                    Replace expected Junit 4 @Test field with assertThatThrownBy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
To simplify a future Junit5 migration this PR removes the usage of the [expected](https://junit.org/junit4/javadoc/4.13/org/junit/Test.html#expected()) field of the `org.junit.Test` annotation with the AssertJ's `assertThatThrownBy` method.

- [HEAD~3](https://github.com/diega/besu/commit/expected_replace~3): Fix two tests from `o.h.b.e.vm.OperandStackTest`, the name of the tests referred to testing `o.h.b.e.internal.OperandStack#set` but they were actually testing _get_ (duplicated indeed, b/c proper tests for _get_ existed with the right method name) -> Thanks @macfarla!
- [HEAD~2](https://github.com/diega/besu/commit/expected_replace~2): Remove unreachable asserts
- [HEAD~1](https://github.com/diega/besu/commit/expected_replace~1): Syntactic wrapping of lines throwing the expected exception
- [HEAD](https://github.com/diega/besu/commit/expected_replace): Extract variables to let only a single method call inside the `assertThatThrownBy` lambda

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 22:54:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3812" class=".btn">#3812</a>
            </td>
            <td>
                <b>
                    cli: Do not warn when using --fast-sync-min-peers with snap sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">snapsync</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The --fast-sync-min-peers option and its value are also relevant for
snap sync. We should therefore not log a warning about the min peers
option being ignored if it is passed.


## Fixed Issue(s)

Fixes #3801

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 08:22:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3811" class=".btn">#3811</a>
            </td>
            <td>
                <b>
                    [MAINTAINERS] new non-code maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I propose adding Helen George and Matt Nelson to Besu non-code maintainers. They have started helping manage, categorize bugs and other Github issues for Besu, as well as collaborating with the existing maintainers to help coordinate the development and roadmap planning of Besu.

Becoming non-code maintainers, they will be able to label bugs and close relevant tickets, helping to keep the project tidy.

Voting ends two weeks from today.

For more information on this process see the Becoming a non-code Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 23:17:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3809" class=".btn">#3809</a>
            </td>
            <td>
                <b>
                    Stop the BlockPropagationManager when it receives the TTD reached event
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3797
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 17:43:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3808" class=".btn">#3808</a>
            </td>
            <td>
                <b>
                    Backward Sync should remember recent finalized blocks.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When syncing using BWS we now consider finalized blocks reported by consensus layer.
When no finalized block is specified, nothing strange will go on. When finalized block is specified
But Besu is not aware of any finalized block yet, we will sync as usual until the finalized block is about to get imported.

A new invariant is introduced when importing blocks using BWS.
All imported blocks have to descent from latest finalized block or a TTD block if we did not finalize yet.

* Importing a finalized block updates the information in Besu Mutable Blockchain.
* It is no longer possible to import blocks into the blockchain below a previously finalized block when using BWS
* When a new finalized block gets announced while BWS is in progress and Besu already has it imported the Mutable Blockchain gets updated, and the chain gets checked for possible pruning
* When trying to import blocks of equal height as newly announced finalized block, then only the new announced finalized block will be possible to import using BWS
* When importing a new block using BWS after finalized, we can now guarantee that the block descends from latest finalized block

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 10:56:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3807" class=".btn">#3807</a>
            </td>
            <td>
                <b>
                    Filter Netty native lib errors likewise the pure Java implementation
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

Since version `22.4.0` Netty prefers the native lib implementation, instead of the pure Java implementation, and this causes warn log messages in case IPv6 is not enable or configured. These error messages are intercepted and logged at debug when thrown by the pure Java implementation, but the native lib implementation triggers a different exception, so the scope of this PR is to extend the error filtering logic to intercept and log at debug the equivalent errors thrown by the native lib implementation

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3798 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 10:54:59 +0000 UTC
    </div>
</div>

