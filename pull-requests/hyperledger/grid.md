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
                PR <a href="https://github.com/hyperledger/grid/pull/1450" class=".btn">#1450</a>
            </td>
            <td>
                <b>
                    Add config object for Griddle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This change adds a 'config' module to Griddle (currently unused) that will be utilized to build the Griddle daemon to run. This allows for config values to be collected from various sources, currently including environment vars, default values, and clap arguments. 

TO-DOs: 
- Add tests 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 15:37:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1449" class=".btn">#1449</a>
            </td>
            <td>
                <b>
                    Add Shutdown trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This change adds a threading module, which contains a lifecycle trait
for handling a thread shut down.

The threading module is available behind the experimental `lifecycle`
feature.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 16:35:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    Add copyright to Griddle's Cargo.toml file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 16:31:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1447" class=".btn">#1447</a>
            </td>
            <td>
                <b>
                    Update maintainer name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Amelia Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 15:49:18 +0000 UTC
    </div>
</div>

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

