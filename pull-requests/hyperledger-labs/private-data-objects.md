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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/463" class=".btn">#463</a>
            </td>
            <td>
                <b>
                    Enable tests in SGX HW-mode (locally)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables tests in SGX HW-mode.

Some important points and things to be discussed:

1.  there appears to be some redundancy between (a) `docker build` and (b) `docker-compose build` in the docker Makefile. When testing in HW mode, it's not clear which build is used and there is discrepancy in using args (e.g., (a) does not pass the `SGX_MODE` variable). Ideally we may want to consolidate the build of the images and just use compose for running tests.

2.  this PR passes the `SGX_MODE` variable to all the builds (particularly those that use it). This is necessary when we build the services, and it's also nice to have since we set the relative env var in the docker file, the env var persists in the image, so later the variable can be used to distinguish between SIM/HW-mode images.

3. `environment.sh` sets `PDO_SGX_KEY_ROOT` to a folder within the `XFER` folder. However, the `XFER` is not available during a docker build (it's docker compose that later mounts that). This is a problem during the service build, because PDO uses that folder to store the enclave signing key. Since the key is ephemeral for now, this PR moves the enclave signing key to `/tmp/`.

4. The policy registration script is called in one of two different places, depending on `SGX_MODE`. Namely: `register-with-ledger.sh` in HW-MODE, and `start_ccf_network.sh` in SIM-mode. First, these calls should be consolidated in a single place (probably the former). Second, `start_ccf_network.sh` and (in particular) the CCF images only need the `SGX_MODE` variable to trigger this script.

5. The policy registration script looks for the CCF keys in multiple places. We should discuss whether the XFER folder is the only reasonable place where these could be, and simplify the rest.

6. Among the global user-facing environment variables, PDO defines `PDO_LEDGER_URL`. However, in multiple places now PDO is using a combination of `PDO_LEDGER_ADDRESS` and (hard-coded) port -- because this is what CCF needs. We should discuss whether address and port should be promoted to global envs, or rather be derived from the ledger url.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 07:36:43 +0000 UTC
    </div>
</div>

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

