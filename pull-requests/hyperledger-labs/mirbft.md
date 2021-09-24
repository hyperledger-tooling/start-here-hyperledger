---
layout: default
title: mirbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/mirbft
---

# mirbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/mirbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Top level refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 13:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Redefine Net module, adding message reception
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The interface of the Net module now contains also a Receive() function,
such that all networking can be encapsulated inside that module.
The option of injecting messages manually (through Node.Step()) still exists
and is an alternative to using the Net module's interface.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 11:46:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Add high level module descriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The /doc directory is now cleaned up and its content moved to legacy_doc.
The new /doc only contains a README.md file with very high-level descriptions
of library architecture and its modules. The main README.md is now also
updated with instructions on how to compile and run tests.

The ClientTracker is now also treated as yet another module.

When the user does not specify certain modules at node instantiation,
defaults will now be used automatically.

Signed-off-by: matejpavlovic <matopavlovic@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 12:03:15 +0000 UTC
    </div>
</div>

