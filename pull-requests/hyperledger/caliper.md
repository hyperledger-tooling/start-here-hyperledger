---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1335" class=".btn">#1335</a>
            </td>
            <td>
                <b>
                    upgraded node-sdk binding for fabric-v2-lts from 2.2.11 to 2.2.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                upgraded to new 2.2 node-sdk that specifies node 16

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 16:46:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1332" class=".btn">#1332</a>
            </td>
            <td>
                <b>
                    Upgraded node-sdk binding for fabric-v1-lts from 1.4.19 to 1.4.20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Node SDK v1.4.20 relaxes the Node version check to >=10.13.0, so should be happy with any later Node version, even though only the LTS releases are “supported”

This upgrade will help remove all the warnings about node versions on caliper.

Signed-off-by: fraVlaca <ocsenarf@outlook.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 10:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1331" class=".btn">#1331</a>
            </td>
            <td>
                <b>
                    disable logging debug to file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To ensure that caliper manager and workers are at their most performant
out of the box, this disables logging debug output to a file

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 16:12:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1330" class=".btn">#1330</a>
            </td>
            <td>
                <b>
                    [Doc] document the new peers property in fabric network config file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also remove references to `type: local` from benchmark files

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 16:03:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1329" class=".btn">#1329</a>
            </td>
            <td>
                <b>
                    add peers property support to fabric network config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add ability to list 1 or more fabric peers in an organisation that can
be used to discover the fabric network. The new Peer Gateway connector
will only ever use the first one (Issue exists to allow for more gateway
peers to be used as load balancers)

This means connection profiles are not needed anymore reducing the
network configuration to a single file (ideally you would embed the
tlsCACert information as well

This will work for
- bound fabric 1.4 using gateway-enabled
- bound fabric 2.2
- bound fabric 2.4

It will not work with bound fabric 1.4 without gateway-enabled and the
connector will report a failure saying that it cannot work with a
dynamic connection profile (there is an issue to enable dynamic profile
support for this but the 1.4 connector is legacy and not worth investing
in)

The implementation works by generating a dynamic connection profile from
the peer information as all the connectors work by working to an
interface which abstracts the required information but the
implementation gets that information by processing an in memory version
of the connection profile and doesn't make sense to have 2 different in
memory representations.

Documentation still to be provided

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 15:08:09 +0000 UTC
    </div>
</div>

