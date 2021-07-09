---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/804" class=".btn">#804</a>
            </td>
            <td>
                <b>
                    Add private fields to Pike store's Role
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the Role struct in the PikeStore to have private fields, with public accessor methods. This PR also adds a `RoleBuilder` implementation that may be used to create a `Role`. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 12:13:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/803" class=".btn">#803</a>
            </td>
            <td>
                <b>
                    Reconnect scabbard event processors on restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To Test:

Start up a network using

```
$ docker-compose -f examples/splinter/docker-compose.yaml up --build
```

Follow the guide for [creating circuits](https://grid.hyperledger.org/docs/0.2/creating_splinter_circuits.html).

`ctrl+c`  the compose run, followed by 

```
$ docker-compose -f examples/splinter/docker-compose.yaml up
```

Attempt to create a role (via the [pike guid](https://grid.hyperledger.org/docs/0.2/using_pike.html))

Before this PR, this would not receive state delta events.  After, the state delta events should still be applied.

~Depends on #801~ 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 21:45:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/802" class=".btn">#802</a>
            </td>
            <td>
                <b>
                    Update default schema owner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This matches the name of the schema owner in the docs

Signed-off-by: Darian Plumb <dplumb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 21:11:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    Add get_current_service_commits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a method to the `CommitStore` to provide the current commits for all services.

It also adds the implementation for the `DieselCommitStore`, supplying the query via an operation trait.  The operation implementation itself requires using a raw SQL query, as the query cannot be generated using the diesel DSL (as of diesel 1.4.x releases).

It is guarded behind the experimental feature `"commit-store-service-commits"`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 15:41:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/800" class=".btn">#800</a>
            </td>
            <td>
                <b>
                    Rename pike to grid_pike
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The rest of the grid contracts are prefixed with grid_, this change updates
pike to match.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 21:14:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/799" class=".btn">#799</a>
            </td>
            <td>
                <b>
                    Add accessor methods to Pike `Agent`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes a few changes in order to allow the fields of the `Agent` Pike struct to be private, rather than public. Store objects should have private fields and accessor methods, hence the change. Also, this PR adds a new `builder` module within the Pike store which currently holds an `AgentBuilder` used to construct agents. This PR also implements the use of the `AgentBuilder`. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 19:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/798" class=".btn">#798</a>
            </td>
            <td>
                <b>
                    Fix just ci recipe
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 19:08:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    Fix various small issues in Pike CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 20:41:36 +0000 UTC
    </div>
</div>

