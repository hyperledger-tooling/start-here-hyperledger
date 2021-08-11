---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1347" class=".btn">#1347</a>
            </td>
            <td>
                <b>
                    feat: set arbitrary plugin config value at cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Doing a bit of spit balling.

We previously addressed the need for supplying configuration to plugins with the `--plugin-config` flag to load a yaml file into `settings` for use by plugins. We've found this feature to be quite helpful, especially in the case of loading multiple plugins (i.e. resolvers) that each require their own configuration. However, we have also found that it would be handy to be able to set or modify these values from the command line. So instead of having to modify the `plugin_config.yml` you're using to load the universal resolver plugin to point it to a different resolver instance, we could have a command line argument like the following:
```
--plugin-config-value http_uniresolver.endpoint=http://localhost:3000
```

Or perhaps a short form of:
```
-o http_uniresolver.endpoint=http://localhost:3000
```

With such a command line argument, we propose that dotted key values act as a shorthand for nesting values. For example, `a.b.c.d=value` becomes `{"a": {"b": {"c": {"d": "value"}}}}`. We also propose that the value be loaded as yaml to avoid parsing ourselves while still allowing us to express values more complicated than just strings and numbers.

Open to thoughts :slightly_smiling_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 00:35:28 +0000 UTC
    </div>
</div>

