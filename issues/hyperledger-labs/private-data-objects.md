---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/private-data-objects/issues/484" class=".btn">484</a>
            </td>
            <td>
                <b>
                    The `warn` method in logging is obsolete and should be replaced with `warning`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good first issue</span>
            </td>
            <td>
                (the title is self-explanatory; issue identified in #483 ; some references are below)

https://github.com/python/cpython/issues/105376
https://docs.python.org/3/library/logging.html#logging.Logger.warning
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 22:29:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/private-data-objects/issues/476" class=".btn">476</a>
            </td>
            <td>
                <b>
                    Copy service availability test from PDO contracts guardian to PDO services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good first issue</span>
            </td>
            <td>
                Current approach for testing availability of the [eps]services is to attempt retrieval of the information from the service through the /info URL. Basically, if the service is running then the operation will succeed. 

However, to accomplish this, we dig through the configuration files looking for host interface and port (using grep). That means that any attempt to override the port or interface will make the test fail.

Recent commit to the [PDO contracts guardian service](https://github.com/hyperledger-labs/pdo-contracts/blob/main/inference-contract/pdo/inference/scripts/guardianCLI.py#L81) adds a "TestService" interface that is part of the service code. That way, we can start the service and then test it using the same command line (meaning that we end up testing the same configuration). This approach should be far more reliable than the current approach.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 16:22:42 +0000 UTC
    </div>
</div>

