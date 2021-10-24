---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1142" class=".btn">1142</a>
            </td>
            <td>
                <b>
                    build: migrate to Yarn v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">dependent</span><span class="chip">good-first-issue-400-expert</span>
            </td>
            <td>
                ### Description

Depends on https://github.com/hyperledger/cactus/pull/1141

**This is an expert level good first issue, meaning that you don't need to know much about Cactus specifically, but you do need to be an expert in configuring build systems/package managers/etc.**

**Yarn V2 is not yet generally available so we have to wait with this issue until it reaches GA. Do not work on this issue before that happens unless you are okay with waiting**

**There's also a branch out there where Peter already performed the migration, but it's currently broken due to a bug in Yarn v2**

Yarn v2 has some performance improvements (among other things) compared to Yarn v1 so we should migrate over as soon as possible (when it hits GA).


### Acceptance Criteria
1. Developer flow has not changed, commands are the same (so that we don't have to re-write half the documentation)
2. If the dev flow must change then the PR must include the new documentation for this and also a migration guide for people who have the old project build working (it's okay to say that they need to delete everything and do a fresh clone - as long as that actually works)
3. No plug and play for now, let's take it one step at a time.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 18:28:49 +0000 UTC
    </div>
</div>

