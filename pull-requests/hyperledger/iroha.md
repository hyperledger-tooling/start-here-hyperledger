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
                PR <a href="https://github.com/hyperledger/iroha/pull/4283" class=".btn">#4283</a>
            </td>
            <td>
                <b>
                    [refactor] #4277: Infallible key pair generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">crypto</span>
            </td>
            <td>
                ### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4277 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Less useless error-handling

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2024-02-15 14:45:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4281" class=".btn">#4281</a>
            </td>
            <td>
                <b>
                    Changed "some-host" to "localhost" in example/config.docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span>
            </td>
            <td>
                ## Description
In one of our config file we had database default address: "some-postgres". Those sample files are for Iroha's beginners to run Iroha as fast as possible. Telling them to change sample configs to run Iroha IMO is not helping them. Also it is making our life harder, because many times somebody was asking about "I'm doing as in instruction and it is not working".

What is more - we have few config files in `example/` directory:
```
ls config*
config.docker  config.postgres.sample  config.sample  config-win.sample
```
in all of config files the host for DB is `localhost`, only in one of them (which I'm changing now) it is `some-postgres`.
- https://github.com/hyperledger/iroha/blob/88de1c6ca640eacf563bc24ae05c11dd14403c38/example/config-win.sample#L5
- https://github.com/hyperledger/iroha/blob/88de1c6ca640eacf563bc24ae05c11dd14403c38/example/config.postgres.sample#L7
- `config.sample` - this is using RocksDB instead of Postgres

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
1. Easier for Iroha's beginners to run example
2. Less work for us with explaining to them where to change config files
3. Consequence in config files
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
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
        Created At 2024-02-14 08:31:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4280" class=".btn">#4280</a>
            </td>
            <td>
                <b>
                    [ci]: Fix pprof-rs Dockerfile and workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

Fix `Dockerfile.glibc` and `iroha2-profiling-image.yml` profiler image build.
### Linked issue

#4083 

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2024-02-13 09:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4279" class=".btn">#4279</a>
            </td>
            <td>
                <b>
                    [ci]: Fix pprof-rs Dockerfile and workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Backport of profiler `Dockerfile.glibc` and `iroha2-profiling-image.yml` (check https://github.com/hyperledger/iroha/pull/4220, https://github.com/hyperledger/iroha/pull/4221, https://github.com/hyperledger/iroha/pull/4250).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 09:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4276" class=".btn">#4276</a>
            </td>
            <td>
                <b>
                    [ci]: Give `config-changes` the role of an automatic label again
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

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Add a clue for detecting configuration changes

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
        Created At 2024-02-13 06:56:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4275" class=".btn">#4275</a>
            </td>
            <td>
                <b>
                    [refactor] #4174: Stop encoding X25519 keys as Ed25519
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">crypto</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

- Key exchanging trait updated with keys associated types
- X25519 keys are now used as a separate type
- `KeyGenOption` now accepts optional generic

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4174 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

More robust type-system, less error-handling, simpler ed25519 code

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2024-02-12 23:14:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4274" class=".btn">#4274</a>
            </td>
            <td>
                <b>
                    [feature] #4083: Profiling support (backport)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport of profiler integration (check #4220, #4221, #4250).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 11:18:55 +0000 UTC
    </div>
</div>

