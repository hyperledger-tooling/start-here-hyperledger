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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Use event bus to send notifications to Admin connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces support for the newly added event bus in ACA-Py to greatly enhance ability to keep admin connections up to date without polling.

Along with these enhancements are improvements to the credentials exchange and presentations exchange features that were not previously possible without an asynchronous notification system. Instead of automatically accepting all credentials and presentation requests, the toolbox plugin now supports sending notifications about newly received credential offers and presentation requests and can wait for input before accepting.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 15:25:12 +0000 UTC
    </div>
</div>

