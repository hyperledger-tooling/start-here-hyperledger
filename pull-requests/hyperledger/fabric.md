---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4861" class=".btn">#4861</a>
            </td>
            <td>
                <b>
                    up go 1.22.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following changes have been made:
- added new possible error based on platform and Go release
- changed the work with [encoding/json](https://go.dev/pkg/encoding/json/) - https://go.dev/doc/go1.22#minor_library_changes. 
`Marshaling and encoding functionality now escapes '\b' and '\f' characters as \b and \f instead of \u0008 and \u000c`.
- The creators of go overmuch with the change of cover work. So far I have turned on the old flag of cover operation - `GOEXPERIMENT=nocoverageredesign`. I will open a question in the go community. Most likely in the next release of go it will be necessary to remove this flag.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 12:32:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4859" class=".btn">#4859</a>
            </td>
            <td>
                <b>
                    add badger as alternative state database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature

#### Description

BadgerDB was added as alternative for GolevelDB state database.
Choosing the better alternative for the GolevelDB was a goal of my research within the paper *"A Journey Towards the Most Efficient State Database For Hyperledger Fabric"*: 

  * [Short version](https://ieeexplore.ieee.org/document/10174970)
  * [Detailed version](https://www.oajaiml.com/uploads/archivepdf/36321188.pdf)

This PR adds Badger because it showed better performance results in comparison with GolevelDB, Bbolt and RocksDB. 

PR satisfies [potential future items of the current Hyperledger Fabric Roadmap](https://wiki.hyperledger.org/display/fabric/Hyperledger+Fabric+Roadmap#:~:text=Replace%20GolevelDB%20with%20faster%20database) where the goal to replace the GolevelDB with faster database is mentioned.
 

#### Additional details

Detailed Hyperledger Fabric performance reports mentioned in the papers above are availiable [here](https://drive.google.com/drive/folders/102_Kgpxsjcog5RNcXPo8MK1dvVYoGODp?usp=sharing). They were made using Hyperledger Caliper tool. The tool was used to measure main performance metrics on HLF peer with default GolevelDB and integrated Badger, Bbolt and RocksDB. More measuring details are described in the aforementioned studies.

To demonstrate Badger's potential advantage over GolevelDB, go benchmarks were added to the packages leveldbhelper and badgerdbhelper respectively. The results measured locally show that Badger has better performance for "*put*" operations than GolevelDB. The output is:

#### GolevelDB
```bash
go test -benchmem -run=^$ -bench ^BenchmarkLevelDBHelper$ github.com/hyperledger/fabric/common/ledger/util/leveldbhelper
goos: darwin
goarch: arm64
pkg: github.com/hyperledger/fabric/common/ledger/util/leveldbhelper
BenchmarkLevelDBHelper/get-leveldb-little-data-10                5452860               189.3 ns/op           108 B/op          4 allocs/op
BenchmarkLevelDBHelper/put-leveldb-10                                673           2768479 ns/op             248 B/op          3 allocs/op
BenchmarkLevelDBHelper/put-leveldb-type-2-10                         415           2560133 ns/op             204 B/op          3 allocs/op
PASS
ok      github.com/hyperledger/fabric/common/ledger/util/leveldbhelper  7.145s
```

#### Badger
```bash
 go test -benchmem -run=^$ -bench ^BenchmarkBadgerDBHelper$ github.com/hyperledger/fabric/common/ledger/util/badgerdbhelper
goos: darwin
goarch: arm64
pkg: github.com/hyperledger/fabric/common/ledger/util/badgerdbhelper
BenchmarkBadgerDBHelper/get-badgerdb-little-data-10          1388515               727.7 ns/op           410 B/op          8 allocs/op
BenchmarkBadgerDBHelper/put-badgerdb-10                           207873              5808 ns/op            1408 B/op         37 allocs/op
BenchmarkBadgerDBHelper/put-badgerdb-type-2-10                171474              7206 ns/op            1477 B/op         37 allocs/op
PASS
ok      github.com/hyperledger/fabric/common/ledger/util/badgerdbhelper 13.984s
```

The changes were tested locally and with GitHub CI/CD.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 19:49:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4858" class=".btn">#4858</a>
            </td>
            <td>
                <b>
                    chore: fix function names in comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change


- Documentation update

#### Description

fix function names in comment

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 13:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4857" class=".btn">#4857</a>
            </td>
            <td>
                <b>
                    Bump github.com/hyperledger/fabric-lib-go to v1.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/hyperledger/fabric-lib-go to v1.1.2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 18:09:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4856" class=".btn">#4856</a>
            </td>
            <td>
                <b>
                    Allow the peer delivery client to select policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Issue: #4847

#### Related issues

#4847
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-12 16:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4855" class=".btn">#4855</a>
            </td>
            <td>
                <b>
                    Fix docs reference version of hyperledger-fabric-ca from 1.4 to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Last LTS version **[release-1.4](https://github.com/hyperledger/fabric-ca/tree/release-1.4)** of **hyperledger-fabric-ca** was abandoned 4 years ago, but the successor version **1.5** has never been present as a candidate in the [public docs page](https://hyperledger-fabric-ca.readthedocs.io/en/latest/). Instead, the hyperledger-fabric-ca team only update **latest** version.

#### Type of change

- Documentation update

#### Description
To adapt **hyperledger-fabric-ca** docs version, rename all references to hyperledger-fabric-ca version **release-1.4** (if present) to **latest**, namely, change https://hyperledger-fabric-ca.readthedocs.io/en/release-1.4 to https://hyperledger-fabric-ca.readthedocs.io/en/latest. Because **hyperledger-fabric-ca** docs version **release-1.4** hasn't been updated for 4 years, and the public maintaining version is **latest**.

#### Additional details

Updated docs is built out for review: https://ethan-li-fabric.readthedocs.io/en/latest/

#### Related issues

#4854 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-11 01:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4852" class=".btn">#4852</a>
            </td>
            <td>
                <b>
                    chore: fix comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 02:03:06 +0000 UTC
    </div>
</div>

