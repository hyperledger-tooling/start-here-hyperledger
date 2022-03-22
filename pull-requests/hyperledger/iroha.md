---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1993" class=".btn">#1993</a>
            </td>
            <td>
                <b>
                    [ci]: Add telemetry to default features. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

- Add telemetry to default features as per @Cre-eD 's request. 
- Update outdated `README.md` files. 

### Issue

None

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Default deployment has support for prometheus metrics

### Possible Drawbacks

Increased binary size. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 06:58:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1989" class=".btn">#1989</a>
            </td>
            <td>
                <b>
                    [fix] #1897: Changed usize to u64/u32 on serde derived structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

In all the locations where a struct derives Serialize or Deserialize usize has been replaced
with either u64 or u32. No instances of isize existed. In the cases where code using the
data required a usize u32 was chosen as the replacement. There is no point in avoiding usize
in the on disk formats if 32-bit platforms can't read and use the values written.

### Issue

Resolves #1897 
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

No chance of crashing due to serializing on 64-bit then deserializing on 32-bit or vice versa.

### Possible Drawbacks

This change limits the size of certain configuration values to 4 billion. Probably a non issue.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 22:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1984" class=".btn">#1984</a>
            </td>
            <td>
                <b>
                    [refactor]: encapsulate access to data model structures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                Signed-off-by: Marin Veršić <marin.versic101@gmail.com><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

This PR encapsulates access to the data model structures and separates internal structure from the API presented. This will bring about separation of concerns and enable us to have the same API for client applications and wasm access through FFI. Namely, this PR encapsulates FFI heavy structures, it doesn't encapsulate structure such as `Identifiable::Id` because they should be easily serialized across FFI and it's unlikely their internal representation will change 

Includes:
* field accessors - custom and derived with `getset`
* builder pattern for structures implementing `Identifiable`
* name deserialization fix - we should be more mindful of all the paths for constructing structures maintaining invariants

I invite you to think whether this modification of the API is a step in a right direction. Additional simplifications should be left for a separate PR

### Issue

Closes  #1982

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-20 19:20:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1973" class=".btn">#1973</a>
            </td>
            <td>
                <b>
                    Smart contract opaque pointers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

1. How to encode data exchanged between smart contract and Iroha(host)?
Since serialization is too expensive (in smart contract size) and relying on the `repr(C)` ABI is not really tenable, the best technique is to use the opaque pointer approach where smart contract is given opaque pointers and a list of functions to read from or modify the object behind the opaque pointer.

2. Where should the allocated objects reside?
Using opaque pointers implies that they are created on the host side (in host's memory space) and given to the smart contract. The problem is that giving control of the host's memory to the wasm module is a potential security issue. Approach where we'll be storing/serializing allocations to the modules linear memory, if possible to implement, would be very complex. That's why I had to introduce another module which smart contract would link against. This module is responsible for allocations and shares it's linear memory with the smart contract. Having them share memories turned out to be problematic because each module would be instantiated with it's own allocator and would step over each other. That is why smart contract needed an implementation of a custom allocator which would forward all (de)allocation requests to the module responsible for handling memory. This also has the added benefit that smart contract no longer has to include allocation logic inside itself and trims a few more bytes of it.

3. There is too many functions for dealing with smartpointers
Having many function signatures bloats the smart contract binary. This can be alleviated by assigning a unique function id to every function(except a few dedicated) and multiplexing them over just one function `_iroha_fn`. 

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 07:40:35 +0000 UTC
    </div>
</div>

