---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1122" class=".btn">#1122</a>
            </td>
            <td>
                <b>
                    Add support for passing custom HTTP headers through
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on https://github.com/hyperledger/firefly-common/pull/41

Adds support for setting a list of HTTP headers to put on the request Context. If an FFResty client is _also_ to pass headers through, it will set all the same headers on any request that it makes.

Example config:

```yaml
api:
  address: 0.0.0.0
  port: 5000
  publicURL: http://127.0.0.1:5000
  passthroughHeaders:
    - X-SuperCoolCustomHeader
plugins:
  blockchain:
    - ethereum:
        ethconnect:
          url: http://127.0.0.1:5102
          passthroughHeadersEnabled: true
```

This would configure FireFly to pass a header named `X-SuperCoolCustomHeader` through from an HTTP request all the way to the Ethereum blockchain connector.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 21:11:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1120" class=".btn">#1120</a>
            </td>
            <td>
                <b>
                    Update example script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 07:00:14 +0000 UTC
    </div>
</div>

