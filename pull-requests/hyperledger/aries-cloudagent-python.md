---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1960" class=".btn">#1960</a>
            </td>
            <td>
                <b>
                    fix: Safely shutdown when root_profile uninitialized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If an exception was thrown during the initialization of the root_profile, we would throw an exception during shutdown and fail to end the process. This would leave ACA-Py running, without accepting/handling any further requests. Adding guards for shutdown code that uses the root_profile should avoid this situation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 15:32:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1958" class=".btn">#1958</a>
            </td>
            <td>
                <b>
                    feat: 00B v1.1 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>

- Putting this as draft, once PR #1940 is approved and merged, I need to make a minor update to use `get_proto_default_version()` and remove `BASE_PROTO_VERSION` from the OOB messages. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-23 22:33:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1957" class=".btn">#1957</a>
            </td>
            <td>
                <b>
                    key type registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes key types pluggable to enable plugins to define and register new ones.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 23:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1956" class=".btn">#1956</a>
            </td>
            <td>
                <b>
                    Feature: enabled handling VPs (request, creation, verification) with different VCs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Enabled handing presentation requests with indy **and** dif
* Enabled handling presentation requests with requests for claims from different JSON-LD VCs (verifier has to create separate submission requirement groups for each claim from different VC) In case, multiple claims should come from the same VC, the descriptors can be included in the same group

* Updated demo/agent_controller to correctly construct presentations.

Signed-off-by: Anastasiia Sivirina [sivirina99@mail.ru](mailto:sivirina99@mail.ru)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 17:26:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1955" class=".btn">#1955</a>
            </td>
            <td>
                <b>
                    did method registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support different did methods in plugins we need to support did method pluggability. This PR changes the default methods to be static and registered into a registry of methods at start-up. This allows plugins to define new did methods that can be registered. The bulk of changes in this PR is updating the current code to use a did method registry.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 20:23:06 +0000 UTC
    </div>
</div>

