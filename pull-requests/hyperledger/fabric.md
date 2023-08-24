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
                PR <a href="https://github.com/hyperledger/fabric/pull/4395" class=".btn">#4395</a>
            </td>
            <td>
                <b>
                    Do not send channel name as part of each message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the new communication infrastructure implementation, as per the RFC [0], the channel name for the entire lifetime of the gRPC stream, is determined at the time of establishing and authenticating the gRPC stream, and therefore there is no need to send the channel name in each message.

[0] https://hyperledger.github.io/fabric-rfcs/text/orderer-v3.html#orderer-to-orderer-authentication-and-communication

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 13:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4393" class=".btn">#4393</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: seek content type header+sig to send full config bl…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Improvement (improvement to code)
- Test update


#### Description

As described in issue #4354


#### Related issues

issue #4354 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 15:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4392" class=".btn">#4392</a>
            </td>
            <td>
                <b>
                    delete ioutil pkg and redundant type casting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ioutil.Discard -> os.Discard
ioutil.NopCloser -> io.NopCloser
delete redundant type casting
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 08:00:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4391" class=".btn">#4391</a>
            </td>
            <td>
                <b>
                    change from ioutil.ReadDir to os.ReadDir
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
        Created At 2023-08-21 12:05:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4390" class=".btn">#4390</a>
            </td>
            <td>
                <b>
                    add/remove orderer docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docs regarding the addition and removal of an orderer to/from existing cluster or channel.

#### Type of change

- Documentation update

#### Related issues

Issue: #4332 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 09:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4387" class=".btn">#4387</a>
            </td>
            <td>
                <b>
                    Fix linter errors
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

A recent commit introduced some linter errors.
This commit corrects the formatting.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-20 08:42:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4386" class=".btn">#4386</a>
            </td>
            <td>
                <b>
                    change from ioutil.TempFile to os.CreateTemp
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
        Created At 2023-08-19 15:17:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4384" class=".btn">#4384</a>
            </td>
            <td>
                <b>
                    change from ioutil.TempDir to os.MkdirTemp
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
        Created At 2023-08-19 06:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4383" class=".btn">#4383</a>
            </td>
            <td>
                <b>
                    change from ioutil.ReadAll to io.ReadAll
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
        Created At 2023-08-19 06:24:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4382" class=".btn">#4382</a>
            </td>
            <td>
                <b>
                    change from ioutil.ReadFile to os.ReadFile
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
        Created At 2023-08-18 22:40:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4381" class=".btn">#4381</a>
            </td>
            <td>
                <b>
                    change from ioutil.WriteFile to os.WriteFile
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
        Created At 2023-08-18 16:51:59 +0000 UTC
    </div>
</div>

