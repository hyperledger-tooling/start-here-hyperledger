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
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/848" class=".btn">#848</a>
            </td>
            <td>
                <b>
                    chore: change npm token name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fix NPM token name in workflow.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 22:14:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/847" class=".btn">#847</a>
            </td>
            <td>
                <b>
                    chore: change lerna param
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add missing param to make lerna no verify access before trying. Best given our token.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 21:57:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    fix: make toasts appear after modal closes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously the toasts that let the user know a credential or contact had been removed were being covered by the common remove modal. This PR addresses that. It's not a perfect fix but since we're looking at swapping toasts out entirely, it'll do for now.

Here's what it looks like:
![toast](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/a74fad74-2f41-4528-a9cf-154a1da5e92a)

# Related Issues

#835

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 21:48:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    chore: ignore pkg format changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Ignore format changes to packages when using lerna. Some times it changes when lerna touches it if depending on if the file has a new-line at the end.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 21:39:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    chore: fix repo url
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fix repo URL reference in packages file.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 21:31:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    chore: auto answer lerna
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Auto-accept lerna prompts so it can run in a CICD pipeline. Was disable for the first run so I could see what it wanted to publish. LGTM.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 21:18:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    feat: update mobile ver details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Updated the UI for the mobile verifier proof details screen. Improved wording, changed some button functionality, changed header and icons.

![image](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/48fd0c90-fdb5-43fd-924e-abf025f8792f)

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [ ] Updated documentation as needed for changed code and new or modified features;
- [ ] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 20:57:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/841" class=".btn">#841</a>
            </td>
            <td>
                <b>
                    chore: update actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Update actions to latest

# Related Issues


# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 13:21:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/840" class=".btn">#840</a>
            </td>
            <td>
                <b>
                    chore: publish oca pkg to npmjs.org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Use lerna to publish `@hyperledger/aries-oca` package with an `alpha` tag with the versioning pattern denoted below. A alpha release will be triggered manually by `workflow_dispatch`.

- 1.0.0-alpha.1
- 1.0.0-alpha.2
- 1.0.0-alpha.3
- ...

Package versions can be incremented by updating the repo tag and version in the `learna.json` file. To reset to a specific version this command can do it for all publishable packages:

```console
npx lerna version 0.0.0 --signoff-git-commit --sign-git-commit --no-private
```

It will create a commit tag `v0.0.0` in this case with the git command `git tag v0.0.0 -m "v0.0.0"` the `-m` option is important (ask me how I know). Without it, the tag will not be recognized. This tag cam be moved around with `git tag v0.0.0 -m "v0.0.0" SHA256` as needed.

To see what lerna will do for the next publication version run:

```console
npx lerna publish --no-private --loglevel=verbose --canary "major" --dist-tag alpha --force-publish
```

Adjust the `--canary "major"` option as needed.


# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-17 00:13:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/839" class=".btn">#839</a>
            </td>
            <td>
                <b>
                    fix: warning on blank photo attr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously if the photo attribute was blank in any credential field, the user would receive a warning.
I've changed the functionality so that if the photo is blank then it will display as an empty text field instead.  

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 19:54:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    feat: updated mobile verifier proof screen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Updated the mobile verifier proof screen. Changed buttons, enlarged QR code

![image](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/2d38b4c8-0bfb-4286-9040-5cdb9037a311)


# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 19:28:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    fix: only send problem report if connectionid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously declining a proof request would cause Bifold to attempt to send a problem report even if the proof request was connectionless, which caused an error. This PR conditionally sends problem reports only if there is a connection.

Here is the relevant code from AFJ core: https://github.com/hyperledger/aries-framework-javascript/blob/38a0578011896cfcf217713d34f285cd381ad72c/packages/core/src/modules/proofs/ProofsApi.ts#L561

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 17:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/834" class=".btn">#834</a>
            </td>
            <td>
                <b>
                    chore: use @hyperledger pkg scope for oca
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

- Use the `@hyperledger` namespace for publishing the oca npm packages;
- Add descript package name;
- Set initial version and description.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 22:45:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    feat: adding border in password field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Adding border on password field to style in different wallets.

![Image_20230615_162759_098](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/69023582/32a70f5a-0579-43a3-a02c-e254efd5445f)

# Related Issues

 "N/A".

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
- [X] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 20:30:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    feat: extracting size from modal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Modal font size updated to follow the standard font defined on theme.

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [X] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [X] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [X] Updated documentation as needed for changed code and new or modified features;
- [X] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 19:36:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    feat: proof details bullet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Changed the proof request details screen to use bullet points instead of horizontal bars to separate proof items:
 
![Screen Shot 2023-06-14 at 2 18 22 PM](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/36937407/5b3c67af-edc9-4362-bbca-70c982c0957d)

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 21:20:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    fix: fixed back button disappearing from biom screen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously in the biometrics screen accessed from the setting menu, when toggling biometrics on/off and entering the incorrect pin, the left header back button would disappear. These changes ensure that it does not disappear.

# Related Issues
Resolves: #823

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 20:40:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    fix: make proof request decline navigate to home screen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Previously, declining a proof request from the scan screen would navigate users to the connection screen, when it should have been navigating them to the home screen. This PR fixes that.

Here it is in action:
![proof_request_navigation](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/ddd0551f-f423-4535-af67-8af4b18fdc15)

# Related Issues

#821 

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 20:35:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/825" class=".btn">#825</a>
            </td>
            <td>
                <b>
                    fix: make whatarecontacts scrollable, add test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Make the WhatAreContacts screen scrollable and remove the Flatlist

Here's what it looks like with max zoom settings:
![what_are_contacts](https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/cc13c038-0844-4a9d-9927-3b79bf69531f)

Here's what it looks like with normal zoom settings:
<img width="284" alt="WhatAreContacts" src="https://github.com/hyperledger/aries-mobile-agent-react-native/assets/32586431/d02719ca-6a04-4650-a728-021d778ecd5f">


# Related Issues

#822

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 17:36:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    fix: make onboarding more a11y friendly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

This PR makes it clear to screen reader users that the skip button on the onboarding screen skips the introduction to the app.

# Related Issues

N/A

# Pull Request Checklist

Tick all boxes below to demonstrate that you have completed the respective task. If the item does not apply to your this PR **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this);
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components;
- [x] Updated documentation as needed for changed code and new or modified features;
- [x] Added sufficient [tests](../__tests__/) so that overall code coverage is not reduced.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

Pro Tip 🤓

- Read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!
- Your PR will likely not be reviewed until all the above boxes are checked and all automated tests have passed.

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 18:50:26 +0000 UTC
    </div>
</div>

