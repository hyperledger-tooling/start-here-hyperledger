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

