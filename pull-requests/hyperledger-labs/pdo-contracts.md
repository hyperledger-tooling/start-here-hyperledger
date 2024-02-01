---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Add docker support for contracts tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Building on the structure used for PDO, this commit adds a recipe for
building a contracts container that can be used for testing of the
contracts and the jupyter interface to the contracts.
    
The structure is similar to the PDO docker support: keys and
configuration variables are shared through the xfer directory. Tools
run in the container build the contracts, run the tests, and also run
a jupyter server.
    
The behavior can be customized through a local makefile that allows
for override of variables. A local environment file can be used to
customize the behavior docker compose.

Run contract tests: cd docker; make test
Run a Jupyter server: cd docker; make jupyter_test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 00:45:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Revert the cmake dependency to ensure that ubuntu 20.04 continues to be supported
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Most client development now assumes ubuntu 22.04. However we want to continue to support 20.04 for the moment. This will make cmake work with ubuntu 20.04 default cmake version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 19:28:49 +0000 UTC
    </div>
</div>

