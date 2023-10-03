---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    ICS-20: Add JSON encoding support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #81 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 05:28:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    feat(transfer): added memo from cosmos spec and tooling to run gen/test of it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
 440190 pts/3    00:00:00 ps
bash-5.2$ make e2e-test
TEST_MNEMONIC="math razor capable expose worth grape metal sunset metal sudden usage scheme" TEST_BROADCAST_LOG_DIR=/home/dz/github.com/hyperledger-labs/yui-ibc-solidity/./broadcast/Deploy.s.sol go test -v ./tests/e2e/... -count=1
=== RUN   TestChainTestSuite
=== RUN   TestChainTestSuite/TestPacketRelay
=== RUN   TestChainTestSuite/TestPacketRelayWithDelay
    coordinator.go:484: delay for recv@3018 5.212113487s
    coordinator.go:494: delay for ack@2018 6.262699139s
    coordinator.go:484: delay for recv@2018 22.614773615s
    coordinator.go:494: delay for ack@3018 40.81390239s
--- PASS: TestChainTestSuite (144.68s)
    --- PASS: TestChainTestSuite/TestPacketRelay (45.91s)
    --- PASS: TestChainTestSuite/TestPacketRelayWithDelay (98.77s)
PASS
ok      github.com/hyperledger-labs/yui-ibc-solidity/tests/e2e  144.710s
bash-5.2$ 
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 22:02:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    feat(dev): added nix to shell into devenv for this repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 20:59:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    04-channel: fix timeout validation in `sendPacket`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 03:50:25 +0000 UTC
    </div>
</div>

