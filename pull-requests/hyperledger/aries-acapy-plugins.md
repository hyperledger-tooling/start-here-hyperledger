---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Add jamshale as maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I would like to become a maintainer of this repo. Mainly so I can merge approved PR's but also to help review code and help make decisions on the direction of this repo.

I plan on working on it for an extended period of time and believe I meet all the requirements to become a maintainer.

@swcurran @WadeBarnes 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 19:10:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Add redis events plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the redis event persistent queue plugin to the repo.

I wanted consistency with other plugins and for all the code to be contained within the plugin definition so i restructured the directory slightly. I didn't make any code changes other than updating the imports.

The demo was broken. I'm still trying to bring it back but it's been more challenging than I thought and I might make another ticket for this. The load tests in the docs directory were also completely broken so I removed them as well. It would be nice to bring them back.

I updated the integration tests to include the relay service and added a few tests. I still think this should be expanded further, but I think it's good enough for now. In some ways it's better than having the demo imho. I added the basicmessage plugin to the integration test agent to help make sure the messages were received. (I think this is ok because they are integration tests)

I left Shaanjot's name as the author on everything but I removed the inner service pyproject files and combined them together so I changed them slightly.

Updated the pydocs to match the ruff requirements and fixed a few unit tests.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 21:21:39 +0000 UTC
    </div>
</div>

