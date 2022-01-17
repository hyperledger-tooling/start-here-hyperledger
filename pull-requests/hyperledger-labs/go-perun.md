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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    Use UnmarshalBinary and MarshalBinary for converting to/from Binary form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR covers step 4 described in #233.

Note: To be merged after #297.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 16:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Add env serializer interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add envelope serializer abstraction, as described in step 2 and step 3 of #233.

In additions to the changes described there,
    1. Modify MsgSerializerTest to use (En|De)codeEnvelopes instead of directly using (En|De)codeMsg functions.
       As the latter are specific to perunio encoding.
    2. Move the generic serializer tests from `wire/test` to `wire/perunio/test` as these tests are specific to perunio serialization format.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 14:56:26 +0000 UTC
    </div>
</div>

