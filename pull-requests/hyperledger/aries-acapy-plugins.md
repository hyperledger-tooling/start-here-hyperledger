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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Repo Management Script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This contains a script for creating scaffolding for a new plugin, managing global dependencies and configuration and common development files.

It's quite a bit simpler than my first attempt. It still contains a new folder where the global files are stored `plugin_globals`, but it doesn't require any additional files from the plugins themselves. It will combine the dependencies and conflicts will be overridden by the global ones. Config sections will just be overriden by the globals (no merging).

There isn't support for plugins to have extra sections currently. They will just be removed. I'm not sure if we want to let plugins be able to do this anyway. Will make things harder to maintain. 

Files in the existing plugins got adjusted slightly. I think these changes could be safely ignored.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 17:45:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/39" class=".btn">#39</a>
            </td>
            <td>
                <b>
                    Proposal to add chumbert of SICPA as a Maintainer of the repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 17:54:34 +0000 UTC
    </div>
</div>

