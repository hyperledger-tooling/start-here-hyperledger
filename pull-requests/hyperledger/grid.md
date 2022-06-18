---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    Update proxy `From` implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Makes 2 smaller updates:

1. Updates `From` implementation for the native `ProxyResponse` struct to be converted to the Actix-Web-defined `HttpResponse`. The impl now validates the response body size before attempting to deserialize it. Previously, it wasn't checking and this resulted in an error. 
2. Add `url` dependency to `proxy-client-reqwest` experimental feature. Previously, this wasn't being pulled in by the proxy-reqwest feature, which resulted in an error if compiling just this feature.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 18:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1445" class=".btn">#1445</a>
            </td>
            <td>
                <b>
                    Update Griddle to use builder pattern on start-up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Updates Griddle to be built and started using the builder pattern, employed throughout Grid and Splinter. This also updates the main function used to start Griddle, behind an experimental `griddle-builder-run` feature, to use the builder for set-up and tear-down. This also updates a few of the arguments passed to Griddle and removes any components that are not planned on being used for Grid v0.4 (i.e., the previous iterations of the batch processor/submitter, database access).


For testing:
1. Start the griddle docker-compose file: 
```
$ docker-compose -f examples/griddle/docker-compose-splinter.yaml up
```

2. Use the 0.4 documentation to create a splinter circuit, create an organization using the Grid container once the circuit is set-up. 

3. Attempt to hit the endpoint `http://localhost:8000/agent?service-id=01234-ABCDE::gsAA` and observe the response you see. You should see a list that contains your `alpha-agent` (or whatever key name used to submit Grid txns) with paging info and a 200 response. You should also see logs from griddle-alpha-Xs and gridd-alpha with the same responses. If you attempt to hit the endpoint `http://localhost:8080/agent?service_id=01234-ABCDE::gsAA`, you should see the same response received from griddle. This validates the rest api is running, and proxying requests as expected. 

4. Ctrl-c to shut down, observe griddle take its last breath. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 18:25:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1444" class=".btn">#1444</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Use ephemeral EC2 runners for building multi-arch docker images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
            </td>
            <td>
                This branch was pushed to upstream rather than my fork to demonstrate that the secrets are in place to allow the job to run. See https://github.com/hyperledger/grid/actions/runs/2492182698 for a successful build of grid-dev.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 03:24:53 +0000 UTC
    </div>
</div>

