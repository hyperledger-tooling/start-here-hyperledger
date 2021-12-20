---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    Fix gitpod download URL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tim Schlagenhaufer <tim.schlagenhaufer@bosch.io>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/696"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 12:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/695" class=".btn">#695</a>
            </td>
            <td>
                <b>
                    aca-py 0.7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                testing new features with 0.7.3 release of aca-py.

- multi ledger support
- disclose features
- monitor revocation

currently in progress and needs changes in the aca-py client as well

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/695"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 09:56:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/694" class=".btn">#694</a>
            </td>
            <td>
                <b>
                    upgrade to java 17
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
        Created At 2021-12-15 16:15:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/693" class=".btn">#693</a>
            </td>
            <td>
                <b>
                    Merge customization file with english localization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I merged the bcgov customization into the English localization so that we can safely delete it. The polish file still has most of the keys from the English one so we need to either delete the keys from there or fully localize them.

 
Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/693"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 10:42:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    Add endorser support WIP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Configure a BPA (optionally) as an Author or Endorser (requires the appropriate settings on the aca-py agents)

Configure connections (optionally) as Author or Endorser

WIP because I was having some issues with the aca-py endpoints (added some tests on the acapy-java-client repo, including a full end-to-end endorser flow).

Note this code is migrated from an older (now closed) PR.


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/692"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 22:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    Optimized runtime variables script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">frontend</span><span class="chip">Infrastructure</span>
            </td>
            <td>
                - Individual actions in script will only be performed when necessary
    - No runtime/environment variable set - no delay
- Improved maintainability (just add future runtime variable names to the pseudo-array)
- Improved POSIX compliance (should run on virtually any Linux based container image - provided that java is installed)

Signed-off-by: Tim Schlagenhaufer <tim.schlagenhaufer@bosch.io>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/691"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 13:21:08 +0000 UTC
    </div>
</div>

