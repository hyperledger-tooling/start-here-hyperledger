---
layout: default
title: sawtooth-lib
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-lib
---

# sawtooth-lib <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-lib){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    Add new traits and structs for the new Publisher design
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The publisher is in charge of returning the next item to publish
to the Supervisor and consensus. It will return the Artifact to
agree upon, for example a block or a batch execution result.
The publisher needs to be able to continue to publish until it is
told to stop. The work may be canceled if the building Artifact
will no longer be valid, for example if the current chain head has changed.

The following design is done with the goal of defining Rust structs that
takes a set of traits. These traits would allow the same publisher structs
 to be used in any situation (e.i. Scabbard or Sawtooth).

A supervisor will use a PublishFactory that will be used to start
the execution. Once started, a PublishHandle is returned that is used
to finish or cancel the publishing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 14:57:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    Add traits for ArtifactCreator and factory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a trait for ArtifactCreator and
ArtifactCreatorFactory which are used for creating
new artifacts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 19:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    Backport 0-6: Fix rust 1.62 lint 
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
        Created At 2022-07-06 18:26:26 +0000 UTC
    </div>
</div>

