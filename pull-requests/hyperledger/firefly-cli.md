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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    Add public-ipfs flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When running FireFly in Gateway mode, it may be desirable to connect to connect to public IPFS peers, rather than operating in a private cluster. This PR adds a new command line flag for that `--public-ipfs`. It is `false` by default.

Also removed some dead code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 14:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    Enable all plugins for gateway mode, allowing data+IPFS for NFT data etc.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly/pull/1037 and https://github.com/hyperledger/firefly/pull/1034
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 03:05:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    fix error reporting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When incorrect file name passed to `ff init --connector-config ` there is no error.  With this PR, the error is reported
```
Error: Failed to load url : 404 : file:///path/to/file.yaml
```
Signed-off-by: John Hosie <john.hosie@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 20:35:21 +0000 UTC
    </div>
</div>

