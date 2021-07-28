---
layout: default
title: aries-acapy-plugin-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugin-toolbox
---

# aries-acapy-plugin-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugin-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Add "echo agent" to integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces a new component for use in integration tests. This component is referred to as the "echo agent" in code. The agent serves only as a collector of messages received over it's static connections and contains no logic for processing messages (so it is "hollow"... so it "echoes"... hence the name lol). This component enables us to simplify test logic and container orchestration, removing circular dependencies between the test runner and the agent under test that required us to start up the tests with `docker-compose up` instead of `docker-compose run tests`. Using the latter, we can now send pytest options such as `-k test_create_connection` and get the status code of executing the tests returned back to the shell.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 18:05:50 +0000 UTC
    </div>
</div>

