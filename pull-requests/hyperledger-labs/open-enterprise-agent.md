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
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/779" class=".btn">#779</a>
            </td>
            <td>
                <b>
                    feat(prism-agent): add multi-tenant wallet self-service capability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">infra</span><span class="chip">shared</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

ATL-6082. Glue all the `PermissionManagement` logic and allow self-service wallet management endpoints. Tenant now can on-board without admin intervention.

Tests will be added in another PR.

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
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
        Created At 2023-11-08 16:05:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/778" class=".btn">#778</a>
            </td>
            <td>
                <b>
                    feat(pollux): Add migrations needed for JWT revocation
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

https://input-output.atlassian.net/browse/ATL-6132
https://input-output.atlassian.net/browse/ATL-6133

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
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 00:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/776" class=".btn">#776</a>
            </td>
            <td>
                <b>
                    feat: Receive/Store Presentation Request
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

Fixes https://input-output.atlassian.net/browse/ATL-5967

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
* [x] If yes to above: I have added tests to cover my changes
* [x] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 21:24:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/775" class=".btn">#775</a>
            </td>
            <td>
                <b>
                    fix: check for active RLS on db application user
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span><span class="chip">connect</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5793. Check for active RLS after running migration and fail during startup if RLS is not active.

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
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
        Created At 2023-11-03 11:47:06 +0000 UTC
    </div>
</div>

