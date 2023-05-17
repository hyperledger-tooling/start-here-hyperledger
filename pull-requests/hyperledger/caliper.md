---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1499" class=".btn">#1499</a>
            </td>
            <td>
                <b>
                    docker monitor remote monitoring bugfix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- Provide a general summary of the pull request in the Title above -->

## Checklist
 - [x]  A link to the issue/user story that the pull request relates to
 - [x]  How to recreate the problem without the fix
 - [x]  Design of the fix
 - [x]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
<!--- What issue / user story is this for -->
#1493 

## Steps to Reproduce
<!--- Provide a link to a live example, or an unambiguous set of steps to -->
<!--- reproduce this bug include code to reproduce, if relevant -->
1. Add target remote docker container to monitoring in test config
2. Run Caliper targeting the remote docker



## Existing issues
<!-- Have you searched for any existing issues or are their any similar issues that you've found? -->
- [x] [Stack Overflow issues](http://stackoverflow.com/tags/hyperledger-caliper)
- [ ] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
- [ ] [Discord history](https://discord.com/channels/905194001349627914/941417677778473031)

<!-- please include any links to issues here -->
[How do I measure the performance of remote docker container in hyperledger caliper?](https://stackoverflow.com/questions/75764196/how-do-i-measure-the-performance-of-remote-docker-container-in-hyperledger-calip)

## Design of the fix
<!-- Focus on why you designed this fix this way, and what was discounted. Do not describe just the code - we can read that! -->
Removed .remote in line 75 of monitor-docker.js, was likely a typo that was just missed since filterName has no property named remote

## Validation of the fix
Ran a remote monitoring with good results
[report.zip](https://github.com/hyperledger/caliper/files/11498024/report.zip)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 12:30:05 +0000 UTC
    </div>
</div>

