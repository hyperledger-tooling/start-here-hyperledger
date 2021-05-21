---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Virtual channels
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #82 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 09:04:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    :boom: [channel] Update NewFundingTimeoutError to return a value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previously, the function returned pointer to an error. Update it to
  return a value.

- It is idiomatic to return error types as values. The change also
  ensures this func is consistent with constructors for other error
  types.

Closes #73.

Signed-off-by: Manoranjith <ponraj.manoranjitha@in.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-16 19:32:00 +0000 UTC
    </div>
</div>

