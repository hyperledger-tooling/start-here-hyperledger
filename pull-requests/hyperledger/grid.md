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
                PR <a href="https://github.com/hyperledger/grid/pull/821" class=".btn">#821</a>
            </td>
            <td>
                <b>
                    Properly wrap pike man pages at 80 characters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 18:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/820" class=".btn">#820</a>
            </td>
            <td>
                <b>
                    Use builder pattern for Batch store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the Batches store to use the builder pattern established in
other stores. This updates the structs with builders and accessor
methods to help stabilize the feature.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 16:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/819" class=".btn">#819</a>
            </td>
            <td>
                <b>
                    Stabilize commit-store-service-commits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the feature "commit-store-service-commits" by removing the feature. The method it guards will now be part of the complete store API for commits, as a result.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 16:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Pre-stabilization fixes for "commit-store-service-commits" feature
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
        Created At 2021-07-13 14:45:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/817" class=".btn">#817</a>
            </td>
            <td>
                <b>
                    Add doc comments for the batch store methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds some brief doc comments to the Batch store methods. These
comments give a brief description of the operation and the arguments for
that function.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 13:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/807" class=".btn">#807</a>
            </td>
            <td>
                <b>
                    Update smart contracts to version 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change is required to make them compatible with the new pike addressing.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 18:57:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/806" class=".btn">#806</a>
            </td>
            <td>
                <b>
                    Add contracts volume to scabbard-cli containers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds the `contracts-shared` volume to the scabbard-cli containers
for the grid on splinter example. This is necessary for the smart
contract upgrade process to work.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 17:36:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    Remove public fields from Pike Organization, Alternate ID, and metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes public fields from the remaining Pike store structs, including Organization, AlternateId, and OrganizationMetadata. The public fields are replaced by public accessor methods. Creating these objects has been replaced by each struct's builder, which are implemented in the PikeStore's builder module. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 15:03:30 +0000 UTC
    </div>
</div>

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

