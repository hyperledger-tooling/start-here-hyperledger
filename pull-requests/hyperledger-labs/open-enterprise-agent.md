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
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/750" class=".btn">#750</a>
            </td>
            <td>
                <b>
                    fix:  all performance tests run succesfully, add group thresholds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">infra</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

This PR fixes all perforrmance tests currently part of the k6 code base. Previously - some didn't work due to issues with the json() serialisation function and there was inconsitency in scenarios and thresholds.
Now - all tests run and pass on a local testing stack (will commit this in a future PR) and use the same defaults for a smoke test

The performance tests have been refactored to share a common scenario but have their own group level thresholds defined. These are just initial definitions and the thresholds have not been tuned with respect to real levels of performance.

Also, this PR introduces a local docker-compose example for running a single tenant stack - with 3 agents - all sharing a single instance of PRISM Node [VDR] 

Two scripts are included for easily running the local e2e tests as well as performance tests.

The performance tests expect a local prometheus instance to be running to push metrics to but will fail gracefully [and run tests anyone] even if it can't push metrics to this local instance of prometheus

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
        Created At 2023-10-09 12:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/749" class=".btn">#749</a>
            </td>
            <td>
                <b>
                    fix: improve performance for background jobs in multitenancy mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">prism-agent</span><span class="chip">connect</span>
            </td>
            <td>
                Signed-off-by: Shailesh Patil <shailesh.patil@iohk.io>

# Overview
Fixes ATL-5773
Previously, background jobs would iterate through each wallet and then query the databases correspondingly for each one. This approach may present performance issues as the number of wallets increases. To address this, the background jobs are now executed as an administrator user, and the wallet context is constructed based on each individual record.


## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
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
        Created At 2023-10-09 10:55:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    docs: add credential definition docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span><span class="chip">mercury</span><span class="chip">build</span><span class="chip">infra</span><span class="chip">connect</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes https://input-output.atlassian.net/browse/ATL-5851

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
        Created At 2023-10-08 23:45:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/747" class=".btn">#747</a>
            </td>
            <td>
                <b>
                    feat: disable cors by default
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

Previously, the helm-chart for deploying the agent always enabled Cross Origin Resource Sharing with a wildcard pattern - which is not a secure default

Now, the helm-chart defaults to a secure (fail securely principle) setting. This means if the user forgets to set this property - the agent is deployed securely

Impact of this change: environments which do not currently set this property that are used for development or are deployed with a need for applications being developed to access resources accross domains - the following values settings need to be added

```
ingress:
   cors:
      enabled: true
      allow_origins: "domain-to-allow.com"
```

Multiple domains can be specified using `,` as a seperator 
A `*` can be used to signal any domain 

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
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [x] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 13:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/746" class=".btn">#746</a>
            </td>
            <td>
                <b>
                    fix(prism-agent): configure APISIX to return CORS headers from Prism Agent endpoints
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

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [x] Bug fixes (non-breaking change which fixes an issue)
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
        Created At 2023-10-05 09:49:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    fix: change repository and name for rest api clients
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

Fixes repository and names for open enterprise agent rest API clients.

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
        Created At 2023-10-04 17:05:02 +0000 UTC
    </div>
</div>

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

