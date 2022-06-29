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
                PR <a href="https://github.com/hyperledger/firefly/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    Deprecate default value for "ffdx"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This default value will be totally removed in v1.1+ due to #878. Deprecating it on the v1.0.x train will give a cleaner migration path forward.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 19:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/881" class=".btn">#881</a>
            </td>
            <td>
                <b>
                    Move SubmitNetworkAction and RootOrg config to Multiparty Manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also added new transaction and operation types for network action.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 20:17:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    Collapse batchpin.Submitter into multiparty.Manager
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
        Created At 2022-06-24 15:42:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/879" class=".btn">#879</a>
            </td>
            <td>
                <b>
                    surface URI as parameter for token mint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 15:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/878" class=".btn">#878</a>
            </td>
            <td>
                <b>
                    Enable non-multiparty namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12).

* Selectively disable managers and routes depending on the features available in a given namespace.
* Move methods that create definitions into the `definitions` package (so it now has the definition "senders" alongside the definition "handlers"). When multiparty is disabled, the senders call directly to the matched handlers without an intermediate broadcast message.

Potential migration-breaking change: the deprecated `dataexchange.type` key no longer has a default of `ffdx`. Older config files that omitted this key will fail to parse. See #882.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 18:34:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/877" class=".btn">#877</a>
            </td>
            <td>
                <b>
                    Remove "namespace" as a query param from all routes
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
        Created At 2022-06-22 21:42:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/876" class=".btn">#876</a>
            </td>
            <td>
                <b>
                    Handle namespace validation at the route level rather than at data manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Data manager is already part of a namespace, so determination of whether the namespace is valid needs to happen earlier in the router, when we're attempting to lookup the proper orchestrator to handle the request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 21:14:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/875" class=".btn">#875</a>
            </td>
            <td>
                <b>
                    Remove namespace param from remaining manager calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)
Follow-on to #864

This removes "namespace" as a param to remaining manager methods (since each manager is already assigned to a single namespace) and adds "namespace" as a param to most database queries (since all queries should be scoped to a single namespace).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 20:09:37 +0000 UTC
    </div>
</div>

