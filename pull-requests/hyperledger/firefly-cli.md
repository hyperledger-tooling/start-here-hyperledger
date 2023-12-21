---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Remove remote-node-url since connector info provided by tezosconnect.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently remote-node-url is required, but accordance to https://github.com/hyperledger/firefly/blob/4645f28a17f6ad813d0a9cbb39ba07d2a5cca795/docs/tutorials/chains/tezos_testnet.md?plain=1#L33C14-L33C30 we should provide tezosconnect.yml in which we have the same section. So left only section from config   

^^ @denisandreenko 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 17:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    Ensuring HexAddress is Wrapped in String format and as HexAddress
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is pr fixes for #230 

@nguyer @awrichar @peterbroadhurst 
I have been able to implement the fix for issue #230 ensure the HexAddress are  wrapped properly please, I would like reviews 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 14:35:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Besu tests created for the  Ethereum firefly Blockchain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is pr fixes for #7 

@nguyer, @awrichar 
New Unit tests have been written for the [Besu package](https://github.com/hyperledger/firefly-cli/blob/main/internal/blockchain/ethereum/besu/genesis.go) in the Ethereum Blockchain. 
These tests  pass successfully
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 08:09:23 +0000 UTC
    </div>
</div>

