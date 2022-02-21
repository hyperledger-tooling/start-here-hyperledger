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
                Issue <a href="https://github.com/hyperledger/cactus/issues/1567" class=".btn">1567</a>
            </td>
            <td>
                <b>
                    ci: enable caching of container image builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span><span class="chip">P3</span>
            </td>
            <td>
                ### Description

As a maintainer I want to make the CI faster and less wasteful so that it's easier to work with it and uses less energy in an attempt to save the planet.

Therefore the CI should check before building images if they were built already, e.g. some kind of shared cache among different executions would be nice because the way it is now, likely 95% of our image builds are producing the same SHAs from scratch every single time which is wasteful and slower than it should be and especially annoying when we get a flaky build fail even though it was passing several times before.

### Acceptance Criteria
1. Given an image SHA, it only ever gets built once on the CI
2. Applies to all of the image builds that we are doing as part of the `build-containers` CI job (10+ images IIRC)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 22:37:44 +0000 UTC
    </div>
</div>

