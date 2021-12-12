---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Fix payload for config endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously the CLI was posting a stringified JSON object to the config endpoint, rather than actual JSON, which caused FireFly to overwrite the entire admin section of the config. This meant that after FireFly re-applies the new config, it just reverts to the default config value for all the admin settings. It was trying to set all of `config.admin` to one big long string. This fix sends _actual JSON_ which allows FireFly to properly patch the config, rather than overwriting the entire section (with a nonsense string)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 22:11:29 +0000 UTC
    </div>
</div>

