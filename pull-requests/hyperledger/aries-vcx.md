---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1073" class=".btn">#1073</a>
            </td>
            <td>
                <b>
                    docs: Update location of aries agents
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
        Created At 2023-11-28 12:16:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    feat(mediator): Better errors for MediatorPersistence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the first part of effort to introduce better structured errors to the mediator. 
We are using this_error library for the same. And designing the error hierarchy/mapping from bottom up. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 08:57:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1071" class=".btn">#1071</a>
            </td>
            <td>
                <b>
                    Add new Wallet trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A new trait for wallet heavily inspired by #1042. Associated types are leveraged to provide flexibility to various implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-27 14:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    refactor: encryption envelope
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - minor refactoring of encryption envelope which came up in progress of improving did-exchange implementation - a lot more can be done here (and will)
- On top of https://github.com/hyperledger/aries-vcx/pull/1069, please merge that first for clean changelog
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-26 21:34:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1069" class=".btn">#1069</a>
            </td>
            <td>
                <b>
                    feature: Derive Display for all aries messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">review:level-2</span>
            </td>
            <td>
                - Derives `Display` trait for all aries messages 
- Removed default Decorators type parameter `D = NoDecorators` - turned out somewhat problematic in conjunction with the custom `Display` proc macro. Not a big price to pay though, only slightly inconveniences developer working in `messages` crate, but not `messages` consumers.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 23:16:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1068" class=".btn">#1068</a>
            </td>
            <td>
                <b>
                    refactor: uniffi project reorganize
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this PR addresses major reorganize of uniffi project in accordance to #1045 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 21:57:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1067" class=".btn">#1067</a>
            </td>
            <td>
                <b>
                    refactor: deprecate mediation crate - include logic directly inside mediator
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
        Created At 2023-11-22 11:10:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1065" class=".btn">#1065</a>
            </td>
            <td>
                <b>
                    feat: Uniffi credential screen
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
        Created At 2023-11-21 20:37:12 +0000 UTC
    </div>
</div>

