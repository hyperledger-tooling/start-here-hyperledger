---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    chore: update minSdkVersion to get the project version or fallback to 21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the react-native wrapper to get the `minSdkVersion` from the project config or fallback to the current hardcoded version.

I'm not entirely sure if anything else is needed but with this change I could get an app running on React Native 0.74. This change would also be needed in othe repos (`@hyperledger/anoncreds-react-native` and `@hyperledger/indy-vdr-react-native` at least) but I'd like to get approval here before spamming the other repos 😄 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 09:30:46 +0000 UTC
    </div>
</div>

