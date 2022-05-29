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
                PR <a href="https://github.com/hyperledger/besu/pull/3886" class=".btn">#3886</a>
            </td>
            <td>
                <b>
                    Test LZ4_COMPRESSION on all RocksDB column families
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                By default, RocksDB uses Snappy compression algorithm, but from[ RocksDB documentation](https://github.com/facebook/rocksdb/wiki/Compression#configuration), we can read that "LZ4 is almost always better than Snappy".

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

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
        Created At 2022-05-23 08:55:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3885" class=".btn">#3885</a>
            </td>
            <td>
                <b>
                    Maintainers: Remove Curators list and move current Curators to emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Curator role (formerly non-code maintainer) has been separated out and described here https://wiki.hyperledger.org/display/BESU/Curators

This PR does 2 things
* move current maintainers that fall under the "non-code" category to emeritus maintainers, since the separate curator role is sufficient for their purposes
* remove the non-code maintainers section and associated process from the MAINTAINERS.md since this is now defined separately here https://wiki.hyperledger.org/display/BESU/Curators

This PR does not change the process for Besu "code" maintainers, rather removes the extra process so that as a result there is only one type of maintainer.

This PR will remain open for comment for 2 weeks unless a majority of current maintainers votes for the same outcome.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 05:33:00 +0000 UTC
    </div>
</div>

