---
layout: default
title: open-enterprise-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/open-enterprise-agent
---

# open-enterprise-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/open-enterprise-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/902" class=".btn">#902</a>
            </td>
            <td>
                <b>
                    fix: remove oas schema format for empty repsonse body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Update tapir definition so that it doesn't render this
```
type: string
format: binary
```

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 14:28:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/901" class=".btn">#901</a>
            </td>
            <td>
                <b>
                    fix(prism-agent): increase http timeout communication channel closing…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                … with read timeout error

# Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-xxxx

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [x] Improvements (misc. changes to existing features)
* [x] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 12:41:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/900" class=".btn">#900</a>
            </td>
            <td>
                <b>
                    build: make docker image only for the server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Make docker image only for the server
Do not make a docker image for 'pollux/lib/anoncreds'

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 10:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/899" class=".btn">#899</a>
            </td>
            <td>
                <b>
                    feat(pollux): add endpoint to revoke a credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

This PR adds a new endpoint that revokes a credential by its id (id from issue credential records table)

Tests will be added in a separate PR withing this epic

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [x] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [x] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 00:29:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    ATL-6026: Update documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">docs</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-xxxx

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [x] My changes require a change to the project documentation
* [x] If yes to above: I have updated the documentation accordingly

### Tests
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 23:49:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    fix(pollux): fix concurrency problem when issuing a credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

When a credential is issued, the part of the code that determines if a new status list should be allocated for a credential, or if an old one will fit, makes two database calls, one for select and one for insert. these calls are happening in a multi-threaded environment, so they need to happen atomically.

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [x] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 20:53:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    docs: update PR template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                ### Description: 
The change is to use a new PR template.

### Context: 
See the related issue. We will try this PR template and work by iteration to improve it. The goal is that it is simple and added-value for the community.

### Checklist: 
- [x] My PR follows the contribution guidelines of this project
- [ ] My PR is free of third-party dependencies that don't comply with HL-Allowlist
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 16:35:41 +0000 UTC
    </div>
</div>

