---
layout: default
title: firefly-perf-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-perf-cli
---

# firefly-perf-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-perf-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    Support for messages and tokens performance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Full support for broadcast/private message/mint/burn/transfer for performance testing

```shell
Commands:
  get_txs, msg_broadcast, msg_private, token_burn, token_mint, token_transfer

Flags:
  -f, --frequency int          Requests Per Second (RPS) of each worker (default 10)
  -h, --help                   help for ff-perf
  -d, --jobDuration duration   Duration of each job done by worker (default 1m0s)
  -l, --length duration        Length of entire performance test (default 1m0s)
      --longMessage            Include long string in message
  -n, --node string            FireFly node endpoint to test (default "http://localhost:5000")
  -r, --recipient string       Recipient for FireFly messages
      --tokenMessage           Attach message to token
      --tokenType string       [fungible nonfungible] (default "fungible")
  -w, --workers int            Number of workers at a time (default 1)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 21:12:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Update README.md
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
        Created At 2022-01-03 19:54:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    New readme
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
        Created At 2022-01-03 18:49:35 +0000 UTC
    </div>
</div>

