---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2324" class=".btn">#2324</a>
            </td>
            <td>
                <b>
                    Adds unrestricted privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Allows users to utilise unrestricted private transactions. This stores the private transaction in the data of the unrestricted privacy precompile address on-chain. The default implementation is unencrypted, further plugin extension points are required to allow the user to encrypt transactions on-chain. 

## mutually exclusive private restriction modes

### Privacy group state
You can not run a node in mixed `unrestricted`/`restricted` privacy modes. There are potential issues with private state and privacy groups. There is only one private state per group, consequently, you could have a mix of private transaction restriction types in the same group. Whilst it's not a problem per se it could lead to confusion and inconsistent state between nodes.

### Flexible privacy groups
Onchain privacy groups are not currently possible with unrestricted transactions.

### CLI options
`--privacy-enabled` and `--privacy-unrestricted-enabled` must be specified to enable this feature. 

## Changelog

- [ ] adds unrestricted privacy 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 13:18:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2322" class=".btn">#2322</a>
            </td>
            <td>
                <b>
                    Orion info in changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added Tessera/Orion info to changelog

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 23:25:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2321" class=".btn">#2321</a>
            </td>
            <td>
                <b>
                    Fix SECP256R1AcceptanceTest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel@io.builders>

## PR description

SECP256R1AcceptanceTest needed to set `SECP256R1` as signature algorithm instance. Because this variable is static and is used in `BesuNode` to [create a key pair](https://github.com/hyperledger/besu/blob/master/acceptance-tests/dsl/src/main/java/org/hyperledger/besu/tests/acceptance/dsl/node/BesuNode.java#L155) it could happen that other tests were using the SECP256R1 signature algorithm by accident becuase of this, depending on the order in which the tests were executed. This caused the acceptance tests to be flaky.
This PR introduces the possibility to set a pre-generated key pair in `BesuNodeFactory`. This allows to set a SECP256R1 key pair without changing `SignatureAlgorithmFactory.instance`, which avoids that other tests can happen to use SECP256R1 when they expect SECP256K1.

## Fixed Issue(s)
reintroduces test which was ignored in #2267 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:32:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2320" class=".btn">#2320</a>
            </td>
            <td>
                <b>
                    non-existent genesis file: clarify error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Add error message and remove reference to GoQuorum options.
```
$ besu --genesis-file=xyz.json
Unable to read genesis file. java.io.FileNotFoundException: /Users/sallymacfarlane/workspace/besu/xyz.json (No such file or directory)

To display full help:
besu [COMMAND] --help
$ besu --genesis-file=bob.json
Unable to read genesis file. com.fasterxml.jackson.core.JsonParseException: Unrecognized token 'bob': was expecting (JSON String, Number, Array, Object or token 'null', 'true' or 'false')
 at [Source: (String)"bob
"; line: 1, column: 4]

To display full help:
besu [COMMAND] --help
$ cat bob.json
bob
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 01:15:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2319" class=".btn">#2319</a>
            </td>
            <td>
                <b>
                    Fix invalid trace_block during self destruct - 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 14:53:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2318" class=".btn">#2318</a>
            </td>
            <td>
                <b>
                    Remove EIP1559 Gas budget calculator implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

The specification of the EIP1559 has changed and no longer requires a specific gasBudgetCalculator implementation. This PR clean the code by removing this unnecessary part of code

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 11:48:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2317" class=".btn">#2317</a>
            </td>
            <td>
                <b>
                    Fork Block Testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add more testing to ensure new fork blocks are configured properly.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-22 22:56:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2315" class=".btn">#2315</a>
            </td>
            <td>
                <b>
                    Magneto hard fork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
Adds the blocks and the changes for the Magneto hard fork.

## Fixed Issue(s)
Fixes #2314 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-22 05:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2313" class=".btn">#2313</a>
            </td>
            <td>
                <b>
                    Upgrade OpenTelemetry to 1.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Upgrades Otel to 1.2.0.

## Fixed Issue(s)
Fixes #2312 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 05:46:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2311" class=".btn">#2311</a>
            </td>
            <td>
                <b>
                    GoQuorum: Gas estimate to cover PMT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If GoQuorum mode and value = 0, modify tx simulator result to return estimate which will cover a PMT transaction

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 23:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2309" class=".btn">#2309</a>
            </td>
            <td>
                <b>
                    remove london support line and add download link for 21.1.6
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
        Created At 2021-05-20 15:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2307" class=".btn">#2307</a>
            </td>
            <td>
                <b>
                    update maintainer rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

These changes are expected to clarify the rules to reach maintainer status. Some edits were made on the voting process, template PR description added, simplified language,...

The PR also adds a new maintainer type in addition to code maintainer to enable people who significantly contribute to the Besu project to be able to access some project management features such as issues triage and assignation.
Some features, expecially when using Zenhub, indeed require a write access on the repository even though the contributor will not make any code changes. But things like assigning a user to an issue requires maintainer role.

See https://github.com/NicolasMassart/besu/blob/maintainer-rules/MAINTAINERS.md for the easier to read rendered doc.

## Approval of this PR

As for the maintainer addition, this PR being a significant change to the process, I require the same rules to be followed:

- [ ] 2 weeks voting period (ends June 3rd 2021)
- [x] at least 3 approvals
- [x] no veto
- [x] absolute majority makes it pass immediately (currently 11 approvals).

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

We need significant and fully involved non-code contributors to be able to fully help us on the project without the need to contribute code to become a maintainer.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 13:57:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2305" class=".btn">#2305</a>
            </td>
            <td>
                <b>
                    add log blooms for quorum private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When private transactions are executed in goquorum compatible mode the receipts of these private transactions are stored in place of the public marker transaction. To make these receipts discoverable by calls that use the bloom filters the blooms filters of the private transactions have to be combined with the blooms of the public transactions in the right places. 

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2304" class=".btn">#2304</a>
            </td>
            <td>
                <b>
                    Add Vijay Michalik to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Vijay has helped the Besu project through contributions to [user questions](https://chat.hyperledger.org/channel/besu?msg=pEvzRqPLYBvDtbX8m), documentation and [managing issues on the project](https://chat.hyperledger.org/channel/besu?msg=sazaeBhiNpY2Nc5Xk).

Voting ends 2 weeks from the publication of this PR.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

## Approval of this PR

As for the maintainer addition, this PR being a significant change to the process, I require the same rules to be followed:

- [ ] 2 weeks voting period (ends June 3rd 2021)
- [x] at least 3 approvals
- [x] no veto
- [x] absolute majority makes it pass immediately (currently 11 approvals).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:18:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2303" class=".btn">#2303</a>
            </td>
            <td>
                <b>
                    Add Sajida Zouarhi to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>
Sajida has started helping manage Github issues and collaborating with the existing maintainers to help coordinate the development of Besu.

Voting ends 2 weeks from the publication of this PR.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

## Approval of this PR

- [ ] 2 weeks voting period (ends June 3rd 2021)
- [x] at least 3 approvals
- [x] no veto
- [x] absolute majority makes it pass immediately (currently 11 approvals).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 07:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2302" class=".btn">#2302</a>
            </td>
            <td>
                <b>
                    errata discovered in 21.1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
A couple quick fixes for bugs I found In scale testing 21.1.6 pending transactions:
* baseFee = null was not handled correctly in PendingTransactions.updateBaseFee for a fork block
* the transaction gas budget calculator was 2x'ing the already 2x'd gasLimit at and past fork block

we should probably write some tests that cover these cases, but it is late and the release is already out there...

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog


- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 03:26:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2301" class=".btn">#2301</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.1.7-SNAPSHOT
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
        Created At 2021-05-19 22:00:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2300" class=".btn">#2300</a>
            </td>
            <td>
                <b>
                    Release 21.1.6
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
        Created At 2021-05-19 21:45:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2298" class=".btn">#2298</a>
            </td>
            <td>
                <b>
                    Added PKI module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adding the PKI module with the initial setup code for keystore configuration.

## Changelog

No need to update the changelog at this moment as this code isn't part of core Besu yet.

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 20:32:13 +0000 UTC
    </div>
</div>

