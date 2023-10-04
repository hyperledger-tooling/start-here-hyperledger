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
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/744" class=".btn">#744</a>
            </td>
            <td>
                <b>
                    feat: store link secret
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

Fixes https://input-output.atlassian.net/browse/ATL-5827

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
        Created At 2023-10-03 12:49:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/743" class=".btn">#743</a>
            </td>
            <td>
                <b>
                    build: add local developement keycloak and init script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

A preparation work for Keycloak integration. This should enable easy local dev Keycloak instance with `realm`, `client` and static `client-secret` initialized.

```bash
PORT=8080 docker-compose -f infrastructure/shared/docker-compose-mt-keycloak.yml --env-file ./infrastructure/local/.env up
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
* [ ] If yes to abovscriptse: I have updated the documentation accordingly

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
        Created At 2023-10-03 09:42:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/742" class=".btn">#742</a>
            </td>
            <td>
                <b>
                    fix: prohibit tenants to use equal api keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
Code cleanup
APIKEY logic doesn't allow to use the same apikey

Fixes ATL-5768

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [x] Bug fixes (non-breaking change which fixes an issue)
* [x] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [x] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [x] My changes can and should be tested by unit and/or integration tests
* [x] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 07:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/741" class=".btn">#741</a>
            </td>
            <td>
                <b>
                    fix: generified generic secret storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
This is a tech debt refactoring needed for link secret storage

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [x] Improvements (misc. changes to existing features)
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
* [ ] My changes can not or do not need to be tested
* [x] My changes can and should be tested by unit and/or integration tests
* [x] If yes to above: I have added tests to cover my changes
* [x] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 16:17:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/740" class=".btn">#740</a>
            </td>
            <td>
                <b>
                    fix(prism-agent): check issuing DID validity when creating a VC offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">castor</span><span class="chip">prism-agent</span><span class="chip">build</span>
            </td>
            <td>
                # Overview
Fixes ATL-4241
Fixes ATL-5573

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [x] Bug fixes (non-breaking change which fixes an issue)
* [x] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
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
        Created At 2023-09-29 13:05:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    fix: upgrade vault and quill versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">shared</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5829

Upgrading to scala `3.3.1`, it seems to have picked up the `InsertMeta` that was marked unused in scala `3.3.0`. This breaks the tests as the implicit makes quill generate a different SQL statement. `InsertMeta` was remove from quill DSL for `VerificationPolicy` to make to generate the same query.

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
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 11:16:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    fix: Integration flow ATL-5777
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">build</span><span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5777

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
        Created At 2023-09-29 10:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/737" class=".btn">#737</a>
            </td>
            <td>
                <b>
                    fix: Adding labels [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5777

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
        Created At 2023-09-28 13:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    fix: Changing yq command [skip ci] ATL-5777
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

Fixes ATL-5777

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
        Created At 2023-09-28 12:47:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/735" class=".btn">#735</a>
            </td>
            <td>
                <b>
                    fix: Renaming values.yml [skip ci] ATL-5777 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                fix: Renaming values.yml [skip ci] ATL-5777 

# Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5777

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
        Created At 2023-09-28 12:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/734" class=".btn">#734</a>
            </td>
            <td>
                <b>
                    fix: Integration flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span><span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5777

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
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 11:14:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/733" class=".btn">#733</a>
            </td>
            <td>
                <b>
                    fix: Separate config for integration flow ATL-5777
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

Fixes ATL-5777

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
        Created At 2023-09-27 16:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/732" class=".btn">#732</a>
            </td>
            <td>
                <b>
                    fix: ensure all defined performance tests compile and run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

This PR fixes all perforrmance tests currently part of the k6 code base. Previously - some didn't work due to issues with the `json()` serialisation function and there was inconsitency in scenarios and thresholds.
Now - all tests run and pass on a local testing stack (will commit this in a future PR) and use the same defaults for a smoke test

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
        Created At 2023-09-27 15:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    fix: Separate config for integration flow ATL-5777
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span><span class="chip">infra</span>
            </td>
            <td>
                Signed-off-by: Milos Backonja <milos.backonja@iohk.io>

feat: ATL-5777 - Refactoring app-set for test

feat: ATL-5777 - Testing app removal with multiple references

feat: ATL-5777 - Adding item back for testing

feat: ATL-5777 - Removing app reference for test

feat: ATL-5777 - Adding config for dev env

# Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-5777

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
        Created At 2023-09-27 15:29:47 +0000 UTC
    </div>
</div>

