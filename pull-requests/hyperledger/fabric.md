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
                PR <a href="https://github.com/hyperledger/fabric/pull/3628" class=".btn">#3628</a>
            </td>
            <td>
                <b>
                    Fix: typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: typos

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 20:49:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3626" class=".btn">#3626</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove kafka from build
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

Remove kafka from Makefile target docker-third-party as we no longer need kafka and zookeeper

#### Related issues

Issue: #3513 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 13:34:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3625" class=".btn">#3625</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove kafka from configtxgen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I0b623279c0de9ed8ccf5f1ae0627297b0485d81f

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Remove kafka from configtxgen

#### Related issues

Issue: #3513 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-05 13:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3623" class=".btn">#3623</a>
            </td>
            <td>
                <b>
                    fix unittest failed case for TestBadConfigOU with go version 1.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

change certs in dir msp/testdata/badconfigou

because these certs file not contains SANs info, it will failed when go version is 1.19(change func alreadyInChain, not bytes equal)

```
  msp_test.go:1448: 
            Error Trace:    /Users/edward/Documents/GitHub/fabric/msp/msp_test.go:1448
                                        /Users/edward/Documents/GitHub/fabric/msp/ouconfig_test.go:32
            Error:          Received unexpected error:
                            sanitizeCert failed the supplied identity is not valid: x509: certificate signed by unknown authority
                            failed getting certificate for [certificate:"-----BEGIN CERTIFICATE-----\nMIIBrTCCAVKgAwIBAgIJAK8/QQKPJc5dMAoGCCqGSM49BAMCMCkxDDAKBgNVBAoM\nA0NPUDEMMAoGA1UECwwDQ09QMQswCQYDVQQDDAJDQTAeFw0xNzA2MjAwOTA5NDBa\nFw0zNzA2MTUwOTA5NDBaMCkxDDAKBgNVBAoMA0NPUDEMMAoGA1UECwwDQ09QMQsw\nCQYDVQQDDAJDQTBZMBMGByqGSM49AgEGCCqGSM49AwEHA0IABLVK0PcjQjZ/pUsW\nY7NHYJSHaPrc7qY/NK9xfLZogZi1axlOz55k6xQH2LIUILffmzXMm3h391Bim3b9\nrPdsvjqjYzBhMB0GA1UdDgQWBBQF5TG4S2XkK6XVtSUW63ppNTN2dTAfBgNVHSME\nGDAWgBQF5TG4S2XkK6XVtSUW63ppNTN2dTAPBgNVHRMBAf8EBTADAQH/MA4GA1Ud\nDwEB/wQEAwIBhjAKBggqhkjOPQQDAgNJADBGAiEAwhPOEE7bfSlDd0WglM1dNHTY\nhU2p/Lx0mgPha/5HW0UCIQCp6q+qL/OEP+mUms6C9nnMSu2eVDZQQ2MJgRNBVHjC\ncw==\n-----END CERTIFICATE-----\n" organizational_unit_identifier:"COP1" ]
            Test:           TestBadConfigOU
--- FAIL: TestBadConfigOU (8.84s)
```


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
        Created At 2022-09-05 08:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3621" class=".btn">#3621</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove kafka from shared config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I1aefd584e0217642c1315544da8eb1e1849ec759

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Remove kafka brokers from shared config

#### Related issues

Issue: #3513 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 10:52:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3619" class=".btn">#3619</a>
            </td>
            <td>
                <b>
                    Update release information in readme and docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Clarify that v1.4 is out of maintenance
- Releases are now periodic rather than every four months.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 16:20:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3618" class=".btn">#3618</a>
            </td>
            <td>
                <b>
                    Update proto dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To include SeekContentType in orderer protobuf

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 14:06:27 +0000 UTC
    </div>
</div>

