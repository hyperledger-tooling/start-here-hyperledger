---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    fix(tools): fix the names of scripts on README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #1520 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 14:56:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1517" class=".btn">#1517</a>
            </td>
            <td>
                <b>
                    test: supply-chain-backend-api-calls fails without config file #1516
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Made it so that the test uses a config that does not specify a config
file path to be parsed by the config service so that it does not depend
on one existing on the file system when the test gets executed.
It works fine without the .config.json file because we anyway configure
everything via code within the test.

This test started failing while I was working on the Jest/Tap co-existence
pull request so it might have something to do with the migration, but it
does not look like it.

Fixes #1516

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-06 23:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1514" class=".btn">#1514</a>
            </td>
            <td>
                <b>
                    fix: openapi validation for keychain-aws-sm plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes tests for endpoints setKeychainEntry, getKeychainEntryV1,
hasKeychainEntryV1 and deleteKeychainEntryV1, each of them with
test cases:
  - Right request
  - Request including an invalid parameter
  - Request without a required parameter

Relationed with #847

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 09:12:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1513" class=".btn">#1513</a>
            </td>
            <td>
                <b>
                    feat(example): make cartrade support more environments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR resolves Issue #1512 .
Some environments (ex. not centos) have problems with fabcar operation, so I want to make cartrade applications available in more environments. To do this, I first introduce minifabric:<https://github.com/hyperledger-labs/minifabric>.

Signed-off-by: Yasushi Takahashi <t-yasushi@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 07:09:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1511" class=".btn">#1511</a>
            </td>
            <td>
                <b>
                    docs(tools): fix/migrate example config generator to ESM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Fixes #1510

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 17:45:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1496" class=".btn">#1496</a>
            </td>
            <td>
                <b>
                    feat(substrate-aio): add ws-port argument
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR allows developers to choose the port where the saio exposes.

However, there is a bug: the substrate connector cannot connect to the saio running on the custom port. Perhaps it is an issue with port exposing?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 14:05:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1492" class=".btn">#1492</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.0.0-rc.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 22:20:51 +0000 UTC
    </div>
</div>

