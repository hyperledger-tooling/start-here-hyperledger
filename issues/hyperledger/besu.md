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
                Issue <a href="https://github.com/hyperledger/besu/issues/2766" class=".btn">2766</a>
            </td>
            <td>
                <b>
                    Clean up deprecation warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                ### Description
Some methods used by Besu are being deprecated and need to be migrated.

There are some easy wins that have simple method name changes e.g. 

https://github.com/hyperledger/besu/blob/main/nat/src/main/java/org/hyperledger/besu/nat/upnp/OkHttpStreamClient.java#L53
https://github.com/hyperledger/besu/blob/main/besu/src/test/java/org/hyperledger/besu/cli/BesuCommandTest.java#L1922

### Steps to Reproduce 
1. Temporarily add `'-Xlint:deprecation'` to `options.compilerArgs` in the project you want to clean up.
2. rebuild and look for warnings!

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 08:48:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2762" class=".btn">2762</a>
            </td>
            <td>
                <b>
                    subcommands do not support --version flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span><span class="chip">P5</span><span class="chip">dev experience</span>
            </td>
            <td>
                ### Description
As a besu dev, I want subcommands to support -V and --version so that I can see version info even when using subcommands. 

### Acceptance Criteria
* version info displays even using subcommand

### Steps to Reproduce (Bug)
1. `besu blocks -V`

**Expected behavior:** [What you expect to happen]

**Actual behavior:** [What actually happens]
```
➜  besu git:(typo) besu blocks import -V
➜  besu git:(typo) besu blocks  -V
➜  besu git:(typo) besu  -V
besu/v21.7.3-dev-2aaa4e53/osx-x86_64/oracle_openjdk-java-11
```
**Frequency:** [What percentage of the time does it occur?]
100%


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 22:23:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2757" class=".btn">2757</a>
            </td>
            <td>
                <b>
                    Add headings to Besu help
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                This can be done with PicoCLI headings https://picocli.info/quick-guide.html#_section_headings

See related ticket about formatting of the help output
https://github.com/hyperledger/besu/issues/541

### Description
As a developer, I want help grouped sensibly so that it's easy to find what I'm looking for.

Suggested groupings:
GraphQL
JSON-RPC HTTP 
JSON-RPC WebSockets
Metrics
Miner
Privacy
Permissions
Tx pool
(everything else can remain ungrouped)

### Acceptance Criteria
* Besu help has headings for related CLI options

### Steps to Reproduce (Bug)
1. besu --help

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 03:28:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2756" class=".btn">2756</a>
            </td>
            <td>
                <b>
                    Add data-path to error message re chain data mismatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                eg if I start besu with default --data-path and I've already forgotten what the default value is, this will save me looking it up. 

### Description
As a Besu user, I want to see the effective data-path in the error message so that I can delete it if switching between networks. 

### Acceptance Criteria
* Actual/effective data-path is printed out in the error message when genesis block mismatch.

### Steps to Reproduce (Bug)
1. Start besu with --network=rinkeby
2. stop besu
3. start besu with --network=ropsten

**Expected behavior:** [What you expect to happen]
```
Supplied genesis block does not match stored chain data in </path/to/data/path/dir>
Please specify a different data directory with --data-path or specify the original genesis file with --genesis-file.
```
**Actual behavior:** [What actually happens]
```
Supplied genesis block does not match stored chain data.
Please specify a different data directory with --data-path or specify the original genesis file with --genesis-file.
```
**Frequency:** 
every time the genesis block doesn't match

### Additional Information


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 03:03:47 +0000 UTC
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

