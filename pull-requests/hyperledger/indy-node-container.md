---
layout: default
title: indy-node-container
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node-container
---

# indy-node-container <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node-container){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    batch with relativ url not working. fixed.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sebastian Schmittner <sebastian.schmittner@eecc.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 10:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Improve Logging 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introducing a lot of changes to the handling of the Logging.
Introducing new variables:
* INDY_NODE_LOG_LEVEL
* INDY_NODE_LOG_STDOUT
* INDY_NODE_LOG_DIR

Closes #68 #74 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 23:35:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Improved testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
This PR adds a regression test for https://github.com/hyperledger/indy-node-container/issues/69 . The test is sub-optimal, since it was observed that sometimes image pass this test but still fail in production after running for a few weeks (probably due to some libsodium version incompatibility). But this test raises the confidence that images will work in an existing network of reference images (configurable, currently ubuntu16)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 22:58:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node-container/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    debian containers adapted to use old ubuntu 16 (crypto) libs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/hyperledger/indy-node-container/issues/69
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 22:02:18 +0000 UTC
    </div>
</div>

