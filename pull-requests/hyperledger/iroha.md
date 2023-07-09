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
                PR <a href="https://github.com/hyperledger/iroha/pull/3687" class=".btn">#3687</a>
            </td>
            <td>
                <b>
                    [refactor] #2398: Add integration tests for query filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Tests</span>
            </td>
            <td>
                ## Description

Add query filtering functionality for the `client_cli` + integration test for pytest suit. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #2398 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

The more tests the better.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] Extend partially tagged (de)serialize for generics
- [x] Make `Raw` tag optional for `PredicateBox`
- [x] Add ability to skip multi-signature checks in `client_cli`: works faster + correctly for our test
- [x] Fix outdated or buggy test in pytest suit + minor refactoring 
- [x] Add test for query filtersing
- [ ] Still have failures from time to time on some test (my guess it's because we use random peer every time for querying and in case of observing peer it might not be updated on time) 

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 15:47:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3686" class=".btn">#3686</a>
            </td>
            <td>
                <b>
                    [fix] #3607: do not allow decoding/deserialization of SignedTransaction in no_std
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                No way to validate signatures (ursa is not available) - no way to enforce the "signatures are valid" invariant

Better to not support the decoding at all

IMO it still makes sense to decode `SignedTransactionCandidate`, as it does not carry invariants (at least I think so?)

Closes #3607

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 09:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3685" class=".btn">#3685</a>
            </td>
            <td>
                <b>
                    [refactor]: move instruction len from data_model into core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

the less functionality we expose in public API the better

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 12:25:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3684" class=".btn">#3684</a>
            </td>
            <td>
                <b>
                    [ci]: add non-workspace projects to dependabot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

mentioned [here](https://github.com/hyperledger/iroha/pull/3676#discussion_r1254235642)

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 10:53:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3683" class=".btn">#3683</a>
            </td>
            <td>
                <b>
                    [refactor] #3672: Replace HashMap with FxHashMap in derive macros
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Closes #3672 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 10:39:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3680" class=".btn">#3680</a>
            </td>
            <td>
                <b>
                    [chore]: #3679 add @DCNick3 to the MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requested in https://github.com/hyperledger/governance/issues/118
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 07:51:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3678" class=".btn">#3678</a>
            </td>
            <td>
                <b>
                    [chore]: add @DCNick3 to the CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 14:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3676" class=".btn">#3676</a>
            </td>
            <td>
                <b>
                    [ci]: update dependabot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 12:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3675" class=".btn">#3675</a>
            </td>
            <td>
                <b>
                    [feature] #3383: Implement a macro that parses a socket address at compile time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Linked issue

Closes #3383 

### Limitations

This can't replace all uses of the existing `socket_addr!` macro, as it parses only literal addresses. Some of the `socket_addr!` usages use an expression as port number: https://github.com/hyperledger/iroha/blob/19984d91c2add850a197050e6cbee52af1bc6fa2/core/test_network/src/lib.rs#L598. Supporting this is possible, but would require a more complicated parser.

As 5/11 usages of the original macro use it, it probably doesn't make sense to merge it without support for variable ports

It also doesn't support hostname addresses, but they are not used anywhere except in the doc-test for the `socket_addr!` macro. Probably fine going without it, but should be relatively easy to implement if needed.

### Checklist

- [x] Parse IPv4 and IPv6 addresses
- [x] Allow usage of arbitrary expressions in port position
- [x] Replace old usages of `socket_addr!` macro

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 11:52:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3669" class=".btn">#3669</a>
            </td>
            <td>
                <b>
                    [ci] #3648: include `docker-compose.*.yml` check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

This PR adds a CI/CD check that `docker-compose.*.yml` files stored in the repo are generated with `kagami swarm` tool. This PR includes updated Docker Compose configurations as well.

### Linked issue

Closes #3648

### Benefits

It will help to be sure that those files are up-to-date, therefore to avoid confusion of any Iroha users.

### Checklist

- [ ] Ensure that the PR covers **all** Docker Compose files that should be covered.
- [ ] Discuss `docker-compose.TML.yml` in the `check.sh`
- [ ] Discuss/ensure that the check runs in the correct time, as described in #3648: selective run on changes in data model / kagami swarm code, etc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 06:56:07 +0000 UTC
    </div>
</div>

