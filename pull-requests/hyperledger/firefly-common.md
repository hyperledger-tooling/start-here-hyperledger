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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Add number to list of allowed JSON input types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I missed this one in the pervious merge when porting over @peterbroadhurst's changes 🙁 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 16:59:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Allow numbers and booleans to be expressed as strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A slight improvement/replacement for https://github.com/hyperledger/firefly-common/pull/21.

See https://github.com/hyperledger/firefly-signer/pull/11

Allows number for non-integer types (fixed/ufixed) that can be specified as non-string
Update boolean support to include true/false strings as an option (all elementary types allow string basically)

These changes also enforce that a schema cannot allow a `boolean` and a `number` for the same field, as an example
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 15:05:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Allow use of FF object schema generator in custom schema defs for anyOf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need a way to be able to define an `anyOf` schema, which fits nicely with the advanced `ffapi` option for returning a Schema directly. This is for the RPC-style APIs of connectors, where they take a bunch of different payloads that all have some common headers.

However, currently this  custom function can't access all the `struct` schema generation features, so you have to go fully manual - which seems wrong. So I've updated the interface.

I believe all uses of this customization in FireFly core were removed perviously, because of this kind of restriction meaning they are were too static. We took the hit on losing the extra info on the API description, in favor of ensuring it stayed up to date. So this PR should also open the door to re-instating that going forwards.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-18 17:34:39 +0000 UTC
    </div>
</div>

