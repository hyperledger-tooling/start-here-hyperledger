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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Do not include the ",omitempty" in the JSON field name
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
        Created At 2022-08-03 21:37:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Add global config entries to common (so not required in other microservices
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
        Created At 2022-08-02 02:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Utility for serializing structs into a JSON Map (or fftypes.JSONObject)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This utility lets you use the standard JSON serialization policy for fields in go structs, to write fields into a map.

This has two uses in FireFly to avoid horrible JSON marshal/unmarshal loops:

1. Combining multiple Go structures from plugins into an extensible JSON body - required in FFTM here https://github.com/hyperledger/firefly-transaction-manager/pull/14
2. Converting from Go structs to an `fftypes.JSONObject`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 13:02:37 +0000 UTC
    </div>
</div>

