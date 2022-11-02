---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    Add commit hash to Github Actions release workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The commit hash is needed to properly tag the correct release branch release commit.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-28 02:56:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    Increase stability by exposing DB connection and pool properties 
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

Exposed database connection properties so we can have automatic connection recycling in production for when connection pools go stale like when Google Cloud SQL does database maintenance about every quarter, sometimes more.

#### Additional details

Similar to the `maxLifetime` configuration property in the [HikariCP](https://github.com/brettwooldridge/HikariCP#essentials) database library, as well as others, providing access to these connection properties adds significant production stability by enabling connection pools to continually refresh themselves. Given that PostgreSQL connections don't garbage collect objects in SQL connections this configurability of connection pools is a requirement for long-term stability of the CA.

#### Related issues

https://github.com/hyperledger/fabric-ca/issues/321

#### Release Note
Exposes operational database connection properties for ease of CA administration and stability.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-27 18:34:12 +0000 UTC
    </div>
</div>

