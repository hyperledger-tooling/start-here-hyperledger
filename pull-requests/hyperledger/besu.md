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
                PR <a href="https://github.com/hyperledger/besu/pull/5639" class=".btn">#5639</a>
            </td>
            <td>
                <b>
                    Update evmtool graalvm build
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

Update EVMTool's GraalVM build
* add new class to reflection config
* move CLI output to be system-err oriented
* make logger in evmtool nop
* exclude some problematic jars from compilation
  - mixed versions of bouncy castle
  - netty initializations of log4j

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 15:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5638" class=".btn">#5638</a>
            </td>
            <td>
                <b>
                    Updates for execution-spec-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Updates needed to keep executing execution-spec-tests
* add withdrawals support
* add access lists to transactions
* accept t8n and b11r CLI args that are zero length or all whitespace
* Enumerate forks in t8n and b11r help
* remove JSON wrapping from t8n transaction RLP

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 21:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5637" class=".btn">#5637</a>
            </td>
            <td>
                <b>
                    Fail fast in case of downgrade done without reverting variables storage
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

#5471 is backward incompatible, and there is a procedure to do before downgrading, but if the procedure is not followed the db becomes inconsistent, to avoid that this PR tries to detect this scenario and fail fast in case it founds a previous migration, giving the user a possibility to retry the rollback procedure.

If an inconsistency is found this log is printed

```
2023-06-23 16:06:21.885+00:00 | main | ERROR | KeyValueStoragePrefixedKeyBlockchainStorage | Inconsistency found when migrating chainHeadHash to variables storage, probably this is due to a downgrade done without running the `storage revert-variables` subcommand first, see https://github.com/hyperledger/besu/pull/5471
chainHeadHash mismatch: blockchain storage value=0x25a5cc106eea7138acab33231d7160d69cb777ee0c2c553fcddf5138993e6dd9, variables storage value=0x8a3d34ff1d0c4e57fad7c5ec2e316cad84e590e38bd93c386a3ade49deb0437f
```

Tested with this scenario:
1. Existing 23.4.1 Besu with already synced db
2. Upgrade to 23.4.3 and variables migrated
3. Downgrade to 23.4.1 *without* running `storage revert-variables` first, got `World State Root does not match expected value, header 0x5eb6e371a698b8d68f665192350ffcecbbbf322916f4b51bd79bb6887da3f494 calculated 0x0ec284a94272bbfe33f8455acb8f182401607bda6b71c75c3d5584d719e7d8e7`
4. Upgrade again to 23.4.3 and then Besu correctly fails to start since inconsistency detected, with the log reported above.
5. Run `storage revert-variables` successfully rollback variables storage
6. Downgrade again to 23.4.1 and this time Besu starts correctly

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 14:21:18 +0000 UTC
    </div>
</div>

