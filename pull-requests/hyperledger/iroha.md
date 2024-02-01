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
                PR <a href="https://github.com/hyperledger/iroha/pull/4246" class=".btn">#4246</a>
            </td>
            <td>
                <b>
                    [ci] #3889: Add docker-compose files run check into iroha2 CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Add community docker-compose files CI check before image pushing
2. Update community docker-compose files

### Linked issue
#3889 

### Benefits
Validate community docker-compose files integrity and serviceability.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 10:32:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4245" class=".btn">#4245</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4097: Fix warp noise in logs
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
        Created At 2024-01-30 09:31:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4240" class=".btn">#4240</a>
            </td>
            <td>
                <b>
                    [refactor] #1981, #4195: Refactor the event filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- rename the `Filter` trait to `EventFilter`
- "manually" implement all the event filters without macros
  - as a consequence, move all the filters to a separate module
- change the filter types naming scheme to be more logical:
  - AccountFilter -> AccountEventFilter (filters the event as a whole: by origin id and event type)
  - AccountEventFilter -> AccountEventMatcher (matches over a type of event)
- flattens the event filter hierarchy (account event is a kind of domain event, but account event filter is not)

### Linked issue

Closes #1981, #4195

### Benefits

- more orthogonal API: only one way to filter for specific filter API (see #4195)
- simpler to navigate and edit due to not using macros (and with less code!)

### Checklist

- [ ] split events into modules mirroring the events API
- [ ] write code documentation about using the new API
- [ ] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 07:40:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4239" class=".btn">#4239</a>
            </td>
            <td>
                <b>
                    [refactor] #4161: rewrite config, _minimally_
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Documentation</span><span class="chip">config-changes</span><span class="chip">Refactor</span><span class="chip">UI</span><span class="chip">python</span>
            </td>
            <td>
                ## Description

TODO

Creating this draft to see the scope of changes and for CI checks.

### Linked issue

Closes #4161 and some others TODO

### Checklist

- [ ] Fill in description of this PR

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 00:39:13 +0000 UTC
    </div>
</div>

