---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Improve mapping of errors on HTTP responses, and log stacks with debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The use of string parsing could be improved, especially as it doesn't work in cases where the `i18n` framework is used with custom non-`FF` prefixes (which we support).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 22:51:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    add option to specify variables in openapi base path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the option to specify base path variables to openapi generation.

E.g.
```yaml
servers:
  - url: http://example.com/{param}
    variables:
      param:
        default: default-value
```

Since the same route object can be used for swagger generation and route handling, I've also added the option to specify a base path and base path parameters to the handler factory so that path parameters can be parsed out of the request url without them needing to be specified in the route object (which would make them appear under the path in the openapi doc).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 13:09:03 +0000 UTC
    </div>
</div>

