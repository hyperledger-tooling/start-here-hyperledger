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

