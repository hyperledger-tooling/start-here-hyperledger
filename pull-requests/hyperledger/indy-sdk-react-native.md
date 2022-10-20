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
                PR <a href="https://github.com/hyperledger/indy-sdk-react-native/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    chore: switch iOS steps, add pod update for existing projects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've tested the behavior from #56 and everything is working ~~as expected~~ mostly as expected, except for when installing in an existing project--the existing podfile.lock will mean 1.15.0 will continue to be installed instead of 1.16.0, even if Indy is given a specific version in the indy-sdk-react-native.podspec. Here's [info from cocoapods](https://guides.cocoapods.org/using/pod-install-vs-update.html#using-exact-versions-in-the-podfile-is-not-enough) on the issue. I've therefore added a step to do a `pod update Indy` to update to the latest version. 

Additionally, the source command should have come before the pod install from #54, so I've flipped those steps. 

Also, removed the --project-directory in place of a `cd ios` since we have two commands to run. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-20 03:06:07 +0000 UTC
    </div>
</div>

