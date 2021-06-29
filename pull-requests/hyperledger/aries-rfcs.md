---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Add dateint representations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is in response to a conversation on rocket chat starting with:
"Hi all, I had a question about the quintessential zero-knowledge proof example of Alice proving that she is over 18 without revealing her DOB - given that current Indy predicates only work on int32s, what is the best way to represent dates in a credential such that they work for predicate proofs?
I had one idea: at first I was trying to go with an approach of number of days since a certain epoch and being able to use common datetime functions to do the calculations, but it seemed rather complicated and there were a lot of subtle issues around timezones, leap seconds, which epoch to choose, etc. The approach I would like to propose is to apply simple modular arithmetic to map a date to an int of the form YYYYMMDD. This would allow easy conversion to int and back to date without any confusion that would result from using time libraries. The only gotchas I can see are that you couldn't represent dates before AD (which seems ok, or they could be negative which also seems ok), and that you'd need to have some error handling if somehow a credential was ever submitted with an invalid mapping eg 20201332 (13th month, 32nd day, etc) - although some error handling on credential issuing should address that. To construct the proof the verifier would just convert today's date minus 18 years to int form, and then check that the int-date DOB on the credential is < that.
What do people think? Ideally I'd like to use a standard date convention so if there's not already one, I could add a proposal to https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0074-didcomm-best-practices/README.md#date-time-conventions (or create a new RFC).
(And I should specify that 32 bit unixtime wouldn't work, as we want to include dates outside of 1901-2038)"

Signed-off-by: Jacob Saur <jsaur@kiva.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 17:10:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Pickup Protocol v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sam Curren <telegramsam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 19:46:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    refactor: update ECDH-1PU info in RFC-334 and RFC-587
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 16:59:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    update proposed rfcs included in aip to accepted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Saw that RFC 0510 and 0646 were still in proposed state, even though they are included in AIP2.0

Not sure what to do with the links in the AIP RFC, as it seems they all use the same commit. Can I just update the link to the newer commit for these two RFCs? No change has been made besides the `proposed` -> `accepted`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 11:38:26 +0000 UTC
    </div>
</div>

