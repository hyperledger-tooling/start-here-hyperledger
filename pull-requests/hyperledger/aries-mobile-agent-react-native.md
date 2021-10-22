---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Add workflow to build for iOS and Android
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Added a GitHub Actions based wrokflow to make sure the application combines for both iOS and Android.

# Related Issues

I thought we could address #92 with two PRs. The first hist to beef up the workflows by demonstrating that the project can compile for both iOS and Android. This will help ensure no breaking changes are included by contributors. The down side, is that it takes about 25 mins for the iOS build to run on GitHub hardware. Not an overly big issue since its all background work.

The second pull request would be to fix all the LINT issues and then add `npm run lint` back into this workflow or another just for listing. It may also be worth adding husky support to run a lint check on commit to not allow un-formatted code to be pushed out in the first place.

**NOTE**: This will burn through allot of build minutes for private repositories. Build minutes on `macOS` are billed at 10x so a 25 min run-time will be 250 minutes. 

# Pull Request Checklist

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [X] Run prettier: `npm run style-format`
- [X] Updated **documentation** for changed code and new or modified features.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 17:46:40 +0000 UTC
    </div>
</div>

