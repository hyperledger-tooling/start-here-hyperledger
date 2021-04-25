---
layout: default
title: caliper-benchmarks
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper-benchmarks
---

# caliper-benchmarks

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger/caliper-benchmarks){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#143](https://api.github.com/repos/hyperledger/caliper-benchmarks/pulls/143)
            </td>
            <td>
                <b>
                    Fix cannot remove mychannel.tx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If you run the following command (forgot to run `generate.sh` first):

```bash
npm init -y
npm install --only=prod @hyperledger/caliper-cli@0.4.0
npx caliper bind --caliper-bind-sut fabric:1.4
npx caliper launch manager --caliper-workspace . --caliper-benchconfig benchmarks/scenario/simple/config.yaml --caliper-networkconfig networks/fabric/v1/v1.4.1/2org1peergoleveldb/fabric-go.yaml
```

You will get an **empty folder** `mychannel.tx` in `networks/fabric/config_solo/`.

After this happens, run `generate.sh` and you will get the following error:

```bash
rm: cannot remove './mychannel.tx': Is a directory
[common.tools.configtxgen] main -> FATA 011 Error on outputChannelCreateTx: Error writing channel create tx: open mychannel.tx: is a directory
```

This problem can be fixed by replacing `rm -f` in `generate.sh` with `rm -rf`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 13:37:50 +0000 UTC
    </div>
</div>

