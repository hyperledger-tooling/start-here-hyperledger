---
layout: default
title: aries-framework-dotnet
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-dotnet
---

# aries-framework-dotnet <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-dotnet){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    Add virtual modifier to all public methods of default services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sebastian Bickerle <sebastian.bickerle@main-incubator.com>

#### Short description of what this resolves:

This PR adds the virtual modifier to all public methods of default services where it was missing. It enables custom services to override the default behaviour or add a custom behaviour. All public methods of default services should have the virtual modifier by default.

#### Changes proposed in this pull request:

- Adds virtual modifier to all public methods of default services

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 10:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    DefaulProofService BuildRevocationStatesFix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Dindexx <kevin.dinh@main-incubator.com>

#### Short description of what this resolves:

Issue where a proof that consists of a combination of attributes with checks for NonRevoked and attributes without checks for NonRevoked couldnt be processed.

#### Changes proposed in this pull request:

Dont build revocation state for attributes where NonRevoked was not set

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 14:44:23 +0000 UTC
    </div>
</div>

