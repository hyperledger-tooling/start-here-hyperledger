---
layout: default
title: yui-docs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-docs
---

# yui-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    Increase sleep duration in Makefile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I followed the instructions in the `samples/minitoken-besu-ethereum` and ran `make setup`, but I encountered the following error. 
By ensuring sufficient sleep time after starting the Blockchain node, I resolved this error. I think this is dependent on the local environment, but there's a possibility that 5 seconds may not be enough.

- My local environment: [MacBook Air (15 inch, M2, 2023)](https://support.apple.com/kb/SP893)

```
$ make setup       
npm run compile

> minitoken@1.0.0 compile
> truffle compile


Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.
go build -o ../build/uly .
docker compose build --no-cache
[+] Building 17.6s (22/22) FINISHED                                                                                                                                                                      
 => [ibc1 internal] load build definition from Dockerfile                                                                                                                                           0.0s
 => => transferring dockerfile: 491B                                                                                                                                                                0.0s
 => [ibc1 internal] load .dockerignore                                                                                                                                                              0.0s
 => => transferring context: 2B                                                                                                                                                                     0.0s
 => [ibc0 internal] load build definition from Dockerfile                                                                                                                                           0.0s
 => => transferring dockerfile: 651B                                                                                                                                                                0.0s
 => [ibc0 internal] load .dockerignore                                                                                                                                                              0.0s
 => => transferring context: 2B                                                                                                                                                                     0.0s
 => [ibc1 internal] load metadata for docker.io/ethereum/client-go:v1.11.6                                                                                                                          2.7s
 => [ibc0 internal] load metadata for docker.io/hyperledger/besu:21.1                                                                                                                               2.7s
 => CACHED [ibc1 1/7] FROM docker.io/ethereum/client-go:v1.11.6@sha256:5d7f40c92c152d7a7da6f1570da468b21d5cb728e91ad281749bf213a1d4a892                                                             0.0s
 => [ibc1 internal] load build context                                                                                                                                                              0.0s
 => => transferring context: 270B                                                                                                                                                                   0.0s
 => CACHED [ibc0 1/6] FROM docker.io/hyperledger/besu:21.1@sha256:0c548b0bd410252129785bacf544f215f1efd7b736c835eaef92fdeef42bafa5                                                                  0.0s
 => => resolve docker.io/hyperledger/besu:21.1@sha256:0c548b0bd410252129785bacf544f215f1efd7b736c835eaef92fdeef42bafa5                                                                              0.0s
 => [ibc0 internal] load build context                                                                                                                                                              0.0s
 => => transferring context: 78B                                                                                                                                                                    0.0s
 => [ibc0 2/6] RUN mkdir -p /tmp/besu/data                                                                                                                                                          0.4s
 => [ibc1 2/7] ADD geth.password /root/geth.password                                                                                                                                                0.0s
 => [ibc1 3/7] ADD genesis.json  /root/genesis.json                                                                                                                                                 0.0s
 => [ibc1 4/7] ADD privatekey  /root/privatekey                                                                                                                                                     0.0s
 => [ibc1 5/7] ADD run.sh  /run.sh                                                                                                                                                                  0.0s
 => [ibc1 6/7] RUN /usr/local/bin/geth --nousb --datadir /root/.ethereum init /root/genesis.json                                                                                                    0.9s
 => [ibc0 3/6] WORKDIR /tmp/besu                                                                                                                                                                    0.0s
 => [ibc0 4/6] ADD ibftConfigFile.json /tmp/besu/ibftConfigFile.json                                                                                                                                0.0s
 => [ibc0 5/6] RUN besu operator generate-blockchain-config --config-file=ibftConfigFile.json --to=networkFiles --private-key-file-name=key                                                        13.9s
 => [ibc1 7/7] RUN /usr/local/bin/geth --nousb account import --password /root/geth.password /root/privatekey                                                                                       8.8s
 => [ibc0] exporting to image                                                                                                                                                                       0.1s
 => => exporting layers                                                                                                                                                                             0.0s
 => => writing image sha256:ec3f036e1648c22123b928b7d4b7ce4d515b0f0d8045ac2ed3b9fc9dd77e938a                                                                                                        0.0s
 => => naming to docker.io/library/chains-ibc1                                                                                                                                                      0.0s
 => => writing image sha256:05361967e06f82162c54c1f117e285bb0b9431df7fde0a9fb8f10d953354730f                                                                                                        0.0s
 => => naming to docker.io/library/chains-ibc0                                                                                                                                                      0.0s
 => [ibc0 6/6] RUN cp ./networkFiles/keys/*/* ./data/                                                                                                                                               0.4s
docker compose up -d
[+] Running 3/3
 ✔ Network chains_default   Created                                                                                                                                                                 0.1s 
 ✔ Container chains-ibc1-1  Started                                                                                                                                                                 0.5s 
 ✔ Container chains-ibc0-1  Started                                                                                                                                                                 0.5s 
sleep 5
npm run migrate:ibc0

> minitoken-besu-ethereum@1.0.0 migrate:ibc0
> truffle migrate --network=ibc0 --compile-none


Compiling your contracts...
===========================
> Compilation skipped because --compile-none option was passed.

/Users/mattsu6666/ghq/github.com/hyperledger-labs/yui-docs/samples/minitoken-besu-ethereum/node_modules/eth-block-tracker/src/polling.js:51
        const newErr = new Error(`PollingBlockTracker - encountered an error while attempting to update latest block:\n${err.stack}`)
                       ^
Error: PollingBlockTracker - encountered an error while attempting to update latest block:
undefined
    at PollingBlockTracker._performSync (/Users/mattsu6666/ghq/github.com/hyperledger-labs/yui-docs/samples/minitoken-besu-ethereum/node_modules/eth-block-tracker/src/polling.js:51:24)
    at processTicksAndRejections (node:internal/process/task_queues:95:5)
UnhandledRejections detected
Promise {
  <rejected> {
    code: -32603,
    message: 'socket hang up',
    data: { originalError: [Object] }
  }
} {
  code: -32603,
  message: 'socket hang up',
  data: { originalError: { code: 'ECONNRESET' } }
}
make: *** [migrate] Error 1
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 05:05:50 +0000 UTC
    </div>
</div>

