---
layout: default
title: indy-sdk-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk-react-native
---

# indy-sdk-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    feat!: update iOS installation to Hyperledger and installation instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR expands upon @niallshaw-absa's efforts in #54, and places the IndySDK framework file and podspec within this Hyperledger repo. I've left the podspec author under @niallshaw-absa, as you performed the majority of the work, but I'd be happy to change this if desired. Again, thank you to your efforts @niallshaw-absa!

Additionally, this PR updates:
* The iOS instructions to include configuring of setting the Bitcode and Build Libraries for Distribution, and notes that Simulators are currently not supported.
* The Android instructions to install Hermes and remove an unnecessary Java import.

If any testing is desired, an essentially identical setup is available using 
```
source 'https://github.com/JamesKEbert/indy-sdk-react-native'
```

I've marked this as a breaking change, as noted by @TimoGlastra in https://github.com/hyperledger/indy-sdk-react-native/pull/54#issuecomment-1217811816
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 19:45:11 +0000 UTC
    </div>
</div>

