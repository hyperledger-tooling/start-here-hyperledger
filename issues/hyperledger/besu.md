---
layout: default
title: besu
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2705" class=".btn">2705</a>
            </td>
            <td>
                <b>
                    Log unused JSON-RPC Request Fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                ### Description
As part of [PR 2690](https://github.com/hyperledger/besu/pull/2690) we allowed all fields in a JSON-RPC call that are not recognized to be ignored.  This was done to support other libraries that would occasionally send "extra" fields (like "type" in eth_estimateGas).  While this increases compatibility, there is a risk we may be unaware of properties that we may want in the future.

To help this, as a node operator I want unknown properties to be appeneded to the console (at info level), including what the field and value is and what type it was trying to be added to.  The particular call would be nice but may be hard to marshal.

One possible approach is to add `@AnySetter` methods in key places and logging the results.  (for context a stackoverflow question: https://stackoverflow.com/a/31164723/8020)

### Acceptance Criteria
Calling any JSON-RPC with an unexpected field will result in the console log notifying me at ~INFO~ DEBUG level.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 16:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2681" class=".btn">2681</a>
            </td>
            <td>
                <b>
                    Update JavaDoc so we can build with Java 16+
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">dev experience</span>
            </td>
            <td>
                Currently Hypedlerger Besu won't fully build when using Java 16 as the JVM that is running the gradle build. One reason is that some of javadoc rules in have changed.

There are two main items that are hitting us
* Not all public classes have comments. Fixing these can be tedious, but it appears our warning setting lets us get away with it.
* Some places we use out-of-order &lt;H3&gt; headings and the javadoc linter really hates that.

If we can get away without adding javadoc on all public methods that would be great.  If we do have to do thousands of javadocs we should consider the bare-minimum needed, without blatently saying "TODO" on all of them. This can be fixed possibly with CLI flags in the build?

The other lint options should be fixed.  The heading order ones in particular.  But if there are syntax and reference bugs those should be fixed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 19:22:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2643" class=".btn">2643</a>
            </td>
            <td>
                <b>
                    [Spike] Determine the tasks required to upgrade from Java 11 to Java 17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span><span class="chip">dev experience</span>
            </td>
            <td>
                This spike should involve an investigation and some initial testing to determine the subtasks required to upgrade Besu to Java 17.
For completion a number of other issues should be created in this epic.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 19:44:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2569" class=".btn">2569</a>
            </td>
            <td>
                <b>
                    Improve error message when verifying enode syntax with xdns-enabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                ### Description

When deploying multiples nodes on private network, the same `BESU_BOOTNODES` env variable is set with all the enodes.
This is ok as a node will detect its own enode.

Now, in a private networking environment such a Kubernetes, the option `BESU_XDNS_ENABLED` is set to true so we can point to the Pods hostnames instead of IPs that will change.

Internally, Besu seems to retrieve from DNS the IP and then substitute it in the enode string.
If any of the nodes listed on the `BESU_BOOTNODES` option is not yet ready, the Kubernetes DNS will not report any IP, and then the Besu command will fail with this message:

```log
Invalid enode URL syntax. Enode URL should have the following format 'enode://<node_id>@<ip>:<listening_port>[?discport=<discovery_port>]'.  Invalid ip address.
```

If the option `BESU_XDNS_UPDATE_ENABLED` is also enabled, Besu does not substitute any IP in the enode string and passes the boot up validations.



**Expected behavior:**

If `BESU_XDNS_ENABLED` is set to true, but `BESU_XDNS_UPDATE_ENABLED` isn't, the error message displayed should be more clear on what is actually happening.

Example:

```
Invalid ip address or DNS query resolved an invalid ip.
```

### Versions
* Software version: `besu/v21.7.1/linux-x86_64/adoptopenjdk-java-11` (docker latest tag at the time of writting).



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 14:20:22 +0000 UTC
    </div>
</div>

