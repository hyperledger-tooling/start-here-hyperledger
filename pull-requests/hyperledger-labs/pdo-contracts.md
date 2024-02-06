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
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Remove unused dependency on Pillow python package from inference cont…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove unused dependency on Pillow Python package while installing inference-contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-05 22:53:22 +0000 UTC
    </div>
</div>

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
Run a Jupyter server: cd docker; make test_jupyter
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 00:45:19 +0000 UTC
    </div>
</div>

