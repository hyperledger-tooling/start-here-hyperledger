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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    Build python wheel for eservice and pservice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">services</span><span class="chip">build</span>
            </td>
            <td>
                This PR replaces the deprecated python .egg package format for the eservice and pservice with the python .whl format. This is achieved by using more recent python build and install tooling.

Blocking #421. Addresses Task 1 of #437 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 23:27:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    Rewrite docker support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rewrite the docker containerization
    
This is a complete rewrite of the dockerization of PDO. This
approach is designed to grealy simplify deployment of containers
for long running services. There are very few management tools
included in the PR (that would be a separate project), but the
documentation includes a fair amount of information on different
patterns of use.
    
Several important differences:
  
* The build process mostly implements the separation of build,
install, configure and run. base dockerfile sets up the basic
build environment; pdo_base and ccf_base build the services and
can be used for development; client, ccf and services are for
running configured containers.

* There is now a single way for passing in the repository that
is used for building. By default it will be created in the directory
where the docker images are built.

* The client is separated from the services for both testing and
deployment. This should improve testing and provide an image for
clients to install to "kick the tires"

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 16:00:03 +0000 UTC
    </div>
</div>

