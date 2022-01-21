---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    Migration guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Documentation describing key considerations when migrating application using the legacy client SDKs to use the Fabric Gateway client API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 18:05:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    Minimise dependencies on Go protobuf versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extract code that depends on a specific protobuf version into a utility package so the main code is agnostic to the protobuf version. This allows the staticcheck rule for deprecated API usage to be enabled for all but that one utility package.

Contributes to #363
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 12:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/373" class=".btn">#373</a>
            </td>
            <td>
                <b>
                    Enable Javadoc build with Java 17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Minor tweaks to Javadoc to satisfy Java 17 parsing enforcement.
- Maven build profile change to avoid using removed Javadoc option with Java 17.
- Remove unused directory and sample yaml.
- Publish build dependency on Docs stage since it publishes Docs artifacts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 18:30:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/372" class=".btn">#372</a>
            </td>
            <td>
                <b>
                    Clean up protobuf compilation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go uses fabric-protos-go so does not need to build protobufs. The protoc command line and Go protoc commands are not required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-14 21:27:03 +0000 UTC
    </div>
</div>

