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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    Upgrade docker images from 20.04 to 22.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Title mostly says it all.  Main trigger was that client docker image had too old a `cmake` to build contracts in `pdo-contracts`.  That said, 20.04 of course is also a bit dated and EOL if in a year.

Tested by running the usual `make test` here and by mounting `pdo-contracts` into a client container and then run `make test` in it (which admittedly initially failed in the inference tests but that was due to the guardian requiring an `apt install libgl1 libcudart11.0` to work properly!   After running that `make test` also worked for pdo-contracts => _Q: should we add these dependencies also to pdo_client.dockerfile?_)

BTW: mounting a pip-cache volume (`docker run -v $(DOCKER_DIR)/cache/pip:/project/pdo/.cache/pip ...`) also sped up greatly testing which made me wonder whehter we couldn't do also some similar caching for build, e.g., to drastically reduce the image build type, in particular for ccf, via [`RUN --mount=type=cache ...`](https://github.com/moby/buildkit/blob/master/frontend/dockerfile/docs/reference.md#run---mounttypecache) but haven't experimented with that yet ...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 03:59:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    Add checks for environment completeness 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                slight modification on code from @g2flyer in PR #462. Separated the environment check into runtime and build time variable checks. Note that this reflects the reality of current dependencies (and we should always be looking for ways to reduce the dependencies). It also does not check for additional variables required for HW mode support.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 16:16:42 +0000 UTC
    </div>
</div>

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

