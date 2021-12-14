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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    Hide sidebar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add runtime environment variables
    - Will be injected when running the BPA container
    - Can be read from frontend code
- Add runtime variables:
    - SIDEBAR_CLOSE_ON_STARTUP: Hides sidebar in UI when opening any frontend page (can still be opened via burger button); "true", "false"
    - SIDEBAR_HIDE_BURGER_BUTTON: Hides the burger button to open/close sidebar independent from above setting; "true", "false"

To hide the sidebar entirely, set both to true e.g. in your docker-compose as environment variables

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/690"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 14:02:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/689" class=".btn">#689</a>
            </td>
            <td>
                <b>
                    Bugfix for CVE-2021-44228 increased Log4J version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Martin Aulich <m.aulich@gmx.de>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/689"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 17:45:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    fix link to local-network scenario
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sy <jasyrotuck@gmail.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/687"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 17:37:57 +0000 UTC
    </div>
</div>

