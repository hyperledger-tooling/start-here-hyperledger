---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1646" class=".btn">#1646</a>
            </td>
            <td>
                <b>
                    adds nat-restrict to cli options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
Adds net-restrict to CLI options (supports Comma-separated array of allowed IP subnets). 

### Issue(s) fixed
<!-- Include the issue number that this PR fixes. {Example: Fixes #123} -->

Fixes #1625 

### Preview
<!-- Provide a PR preview link to the page(s) changed. {Example: https://besu-docs-git-100-branch-hyperledger.vercel.app} -->

- 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 12:15:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1644" class=".btn">#1644</a>
            </td>
            <td>
                <b>
                    fixes 1611: adds page for boilerplate config  and clarifies profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
Simplifies profile explainer
Creates page for input from devs -- to describe most important boilerplate config settings
Small proofs to the CLI page

### Issue(s) fixed
Fixes #1611
Fixes #1623 

Fixes #

### Preview
<!-- Provide a PR preview link to the page(s) changed. {Example: https://besu-docs-git-100-branch-hyperledger.vercel.app} -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 13:55:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1643" class=".btn">#1643</a>
            </td>
            <td>
                <b>
                    adding in some details re the peering process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
Adding in some details regarding the peering process to make it easier to follow


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 10:46:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1642" class=".btn">#1642</a>
            </td>
            <td>
                <b>
                    Add rocksdb and trie-log subcommands to storage command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following https://github.com/hyperledger/besu-docs/pull/1640

Preview: https://besu-docs-git-fork-siladu-storage-subcommand-hyperledger.vercel.app/development/public-networks/reference/cli/subcommands#storage

Here's the relevant cli help for more context...

```
besu storage --help
Usage: besu storage [-hV] [COMMAND]
This command provides storage related actions.
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  revert-variables      This command revert the modifications done by the
                          variables storage feature.
  rocksdb               Print RocksDB information
  trie-log, x-trie-log  Manipulate trie logs
  revert-metadata       Revert database metadata to previous format
  ```
  
  ```
besu storage rocksdb --help
Usage: besu storage rocksdb [-hV] [COMMAND]
Print RocksDB information
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  usage    Print disk usage
```
  
```
besu storage trie-log --help
Usage: besu storage trie-log [-hV] [COMMAND]
Manipulate trie logs
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  count   This command counts all the trie logs
  prune   This command prunes all trie log layers below the retention limit,
            including orphaned trie logs.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 03:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1641" class=".btn">#1641</a>
            </td>
            <td>
                <b>
                    Copy edits for consistency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
<!-- Briefly describe the changes made in your pull request (PR) below. -->

-  Fixes inconsistency in styling for doc

### Issue(s) fixed
<!-- Include the issue number that this PR fixes. {Example: Fixes #123} -->

Fixes #

### Preview
<!-- Provide a PR preview link to the page(s) changed. {Example: https://besu-docs-git-100-branch-hyperledger.vercel.app} -->

-  [Preview](https://besu-docs-git-minor-style-edits-hyperledger.vercel.app/development/public-networks/how-to/bonsai-limit-trie-logs)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 11:16:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1640" class=".btn">#1640</a>
            </td>
            <td>
                <b>
                    Promote x-trie-log subcommand to trie-log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## Description
<!-- Briefly describe the changes made in your pull request (PR) below. -->

Following https://github.com/hyperledger/besu/pull/7278 this renames "x-trie-log" to "trie-log"

### Issue(s) fixed
<!-- Include the issue number that this PR fixes. {Example: Fixes #123} -->

Fixes #

### Preview
<!-- Provide a PR preview link to the page(s) changed. {Example: https://besu-docs-git-100-branch-hyperledger.vercel.app} -->

- 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 06:43:37 +0000 UTC
    </div>
</div>

