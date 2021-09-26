---
layout: default
title: aries-staticagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-staticagent-python
---

# aries-staticagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-staticagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.9.0-pre3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.9.0-pre3
                </span>
            </td>
            <td>
                This pre-release introduces significant changes to several components of the Static Agent library. In general, these changes are intended to simplify the library and make use of existing libraries. In particular, one of the biggest changes of note is that the Static Agent library now uses Pydantic for its Message class with base classes designed to be trivially extended to define more specific messages.

Additionally, the module routing mechanism was simplified. Now, instead of magic values being set on methods in a class and then scrapped from a listing of all attributes of the class, a class var `ModuleRouter` is now used to capture routes.

Finally, the last large breaking change of this pre-release is the renaming of the `StaticConnection` class to just `Connection`. This more clearly represents the purpose and function of the class. The "static" nature of the static library is not derived from the connection somehow behaving differently but rather how that connection is created and stored or otherwise. To elaborate, the `Connection` class could be just as usable in the context of a "thick" agent as it is in a static agent. In such an agent, these connections would be hydrated and dehydrated on demand according to the function of the agent but there's no reason for the `Connection` to look different in this scenario when compared to a static scenario.

Various smaller fixes have also been made. A full accounting will be provided on release.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-staticagent-python/releases/tag/v0.9.0-pre3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-09-26 01:34:33 +0000 UTC
    </span>
</div>

