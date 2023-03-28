---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    CRUD utility for building microservices on the DB layer, and BigInt query fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There's a lot of boilerplate still needed when building a microservice on top of `firefly-common` DB utilities.

This hasn't been addressed in FireFly Core, because so few of the collection are completely "standard", they need all kinds of special tweaks on a per collection basis. So the code is justified.

But in microservices like EVMConnect trying to pick up the framework, it would be great to just define the metadata of the collection and get the basic set of functions for free.

... so here's what's needed after this change (for SQL based DBs at least) - much better I hope:
https://github.com/hyperledger/firefly-common/blob/0d471d9d062ec110bd6426472a524e4ab2b8d440/pkg/dbsql/crud_test.go#L62-L96

I also found there was no `BigIntField` definition in the query support of `ffapi` - which seemed like a bad omission, particularly las we store the DB data in hex. A follow-on change would be needed in FF Core to pick that up for all `FFBigInt` fields

> In draft as I have a little remaining test coverage to close out on
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 17:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Make common version library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've got this copied and pasted around. Felt like it should be a common utility.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 09:08:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Add text/plain content type support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Useful for APIs that relies on envelope based authentication, for instance in many decentralized identity frameworks, which may become part of FireFly in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 16:15:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    improvements for metrics 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Here is the list of improvements:
- Added go and cpu metrics as default
- added more documentation on how the terms used in function names are used in a real metrics string
- added a way to add a component label for all metrics so that we can separate the same metrics (e.g. HTTP requests) of different components
- allowed more chars to be used in the name string
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 14:09:19 +0000 UTC
    </div>
</div>

