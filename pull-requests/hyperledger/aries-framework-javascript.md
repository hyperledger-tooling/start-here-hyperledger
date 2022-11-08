---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1086" class=".btn">#1086</a>
            </td>
            <td>
                <b>
                    refactor: remove dependency on indy ledger service from sov did resolver/registrar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolves: #1066  and  #1067 
Signed-off-by: Sai Ranjit Tummalapalli <sairanjit5@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-06 07:54:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1085" class=".btn">#1085</a>
            </td>
            <td>
                <b>
                    fix(connections): do not log AgentContext object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In last [Aries Framework JS call](https://wiki.hyperledger.org/display/ARIES/2022-11-03+Aries+Framework+JS+Meeting+notes) @niall-shaw reported performance issues when accepting multi-use invitations. 

I've experienced the same issue after migrating to 0.3.0-alpha.x and it turns out that it was happening because some methods in `DidExchangeProtocol` were logging the whole messageContext object, which now includes agentContext and blocks the console for several seconds. This can be avoided by either logging in INFO mode or customizing the logger being in use to only output a certain depth level of objects.

This PR makes a quick-fix of this issue by logging only messageContext.message, to be consistent with other methods from `ConnectionService`. Not sure if it's really useful though, but that's another subject to discuss 😄 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 22:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1084" class=".btn">#1084</a>
            </td>
            <td>
                <b>
                    ci: use graph-type all for lerna publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CD is broken since #1082 has been merged, and it seems that it's because lerna is using alphabetical order when publishing packages (`lerna publish` command), so attempts to build action-menu before core (marked as peerDependency).

According to [Lerna Publish documentation](https://github.com/lerna/lerna/blob/main/commands/publish/README.md#--graph-type-alldependencies), this is because lerna uses by default a `dependencies` graph-type, which will take into account only packages listed in dependencies to determine the build order. As in this case it is listed in peerDependencies, an `all` graph-type must be used.

Another option of course would be to modify action-menu's package.json to set core as a direct dependency. However, this would be also needed for any other package that comes before to core in alphabetical order (such as `bbs-signatures`). I'm not sure if this would be conceptually correct (this was discussed recently [when extracting BBS module](https://github.com/hyperledger/aries-framework-javascript/pull/1035#discussion_r989228931)).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 11:05:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1083" class=".btn">#1083</a>
            </td>
            <td>
                <b>
                    chore: update extension module sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some long-awaited (?) updates to the extension module sample:

- Update README with registration as of AFJ core 0.3.0
- Add DummyModuleConfig to illustrate custom module configuration
- Add an E2E test to be run along the general suite
- Fix demo, as it stopped working somewhere in 0.2.x (most likely related to #1025; more details to be analyzed there) 

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 04:26:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1082" class=".btn">#1082</a>
            </td>
            <td>
                <b>
                    chore: make action-menu and question-answer public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-01 23:14:00 +0000 UTC
    </div>
</div>

