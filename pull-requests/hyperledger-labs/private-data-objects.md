---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    Some minor docker improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A few minor improvements in docker code to
- make tagging more consistent between docker & docker-compose
- allow for client shell to scale to your terminal
- define a few more env variables for client
- some additional docker stop make targets

BTW: in readme i've noticed we suggest in our examples to put user-name into container names. This seems a wise idea for multi-user settings. Should we also adopt it in the makefiles?  Easy to do but haven't changed it yet as i'm not sure if some other places count on the container names being what they are ...

PS: What still happens right now is that depending on whether end containers are built via docker or docker-compose they will result in slightly different builds. Dont think anything is truly funcitonally different, primarily a space and build time-issue, although might be worth while maybe eventually use docker-compose build instead of docker build for building the "leaf-containers"? (With current setup, base containers always have to be built via docker although one could in principle also adopt docker-compose to build them so we could consistently build everything with docker-compose? Though  probably not worth the effort ...)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 20:05:32 +0000 UTC
    </div>
</div>

