---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1051" class=".btn">#1051</a>
            </td>
            <td>
                <b>
                    Migrate from clap to structopts for cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                https://jira.hyperledger.org/browse/IR-1082
Signed-off-by: i1i1 <vanyarybin1@live.ru>


### Description of the Change

This pr migrates from using clap for parsing cli arguments to structopt crate. Also it introduces simple queries for accounts, assets and domains.

### Benefits

There will be typesafe descriptive structures for cli arguments which remove all boilerplate code. It will also let us easier add new commands to cli and manage existing ones. Apart from that it would be more error prune than our previous implementation.
Also now we are able to query domains, accounts, and assets via cli.

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-06 17:10:33 +0000 UTC
    </div>
</div>

