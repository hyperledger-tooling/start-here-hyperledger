---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1577" class=".btn">#1577</a>
            </td>
            <td>
                <b>
                    test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-17 04:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1576" class=".btn">#1576</a>
            </td>
            <td>
                <b>
                    Typo fix in fix-load documentation 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">PR/change requested</span><span class="chip">documentation</span>
            </td>
            <td>
                Fix [1471](https://github.com/hyperledger/caliper/issues/1471)  
## Checklist
 - [x] A link to the issue/user story that the pull request relates to

## Existing issues
- [x] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
<!-- please include any links to issues here -->

#1471 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 15:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    Grafana correction in caliper documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix [1437](https://github.com/hyperledger/caliper/issues/1437)  
## Checklist
 - [x] A link to the issue/user story that the pull request relates to

## Existing issues
- [x] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
<!-- please include any links to issues here -->

#1437 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 03:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    Implement part of #1557: Add tests for replayRate controller.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #1557 
## Checklist
 - [X]  A link to the issue/user story that the pull request relates to
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?

## Issue/User story
Add tests for replayRate controller.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 13:47:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1572" class=".btn">#1572</a>
            </td>
            <td>
                <b>
                    Add tests for `rate-control/compositeRate.js`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- Provide a general summary of the pull request in the Title above -->
This PR aims to create unit-tests for `compositeRate.js` class within our `caliper-core` package.

However, the current tests are failing due to following reasons.

Within our `packages/caliper-core/lib/worker/rate-control/compositeRate.js`, we find the following line : 

https://github.com/hyperledger/caliper/blob/21a98f496c850840c211a670c32fcfa9240612bb/packages/caliper-core/lib/worker/rate-control/compositeRate.js#L76


However, I tried logging out `this.options` and was returned with an empty Object as output. 

```javascript
console.log('Options: ', this.options);
let weights = this.options.weights;
let rateControllers = this.options.rateControllers;
```

I was returned with following logs : 

```markdown
Options:  {}
2024.05.12-00:43:27.856 error [caliper] [composite-rate-controller]     Weight and controller definitions must be arrays.
      2) should throw error when weights and rateControllers lengths are not the same
(Similar errors for other tests too)
```

Due to this our initial check at line 86, that is : 

https://github.com/hyperledger/caliper/blob/21a98f496c850840c211a670c32fcfa9240612bb/packages/caliper-core/lib/worker/rate-control/compositeRate.js#L79

Always throws an error. However, if we replace the line 76 above with 
```javascript
let weights = this.testMessage.content.weights;
```

Then, our tests pass.

What would be the most optimum fix for such cases?

## Checklist
 - [x]  A link to the issue/user story that the pull request relates to 
 - [ ]  How to recreate the problem without the fix
 - [ ]  Design of the fix
 - [ ]  How to prove that the fix works
 - [ ]  Automated tests that prove the fix keeps on working
 - [ ]  Documentation - any JSDoc, website, or Stackoverflow answers?


## Issue/User story
<!--- What issue / user story is this for -->

## Steps to Reproduce
<!--- Provide a link to a live example, or an unambiguous set of steps to -->
<!--- reproduce this bug include code to reproduce, if relevant -->
1.
2.
3.
4.


## Existing issues
<!-- Have you searched for any existing issues or are their any similar issues that you've found? -->
- [ ] [Stack Overflow issues](http://stackoverflow.com/tags/hyperledger-caliper)
- [ ] [GitHub Issues](https://github.com/hyperledger/caliper/issues)
- [ ] [Discord history](https://discord.com/channels/905194001349627914/941417677778473031)

<!-- please include any links to issues here -->
This issue is a small part of #1557 which aims to increase overall code-coverage for the `caliper-core` package.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-11 19:17:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1571" class=".btn">#1571</a>
            </td>
            <td>
                <b>
                    FIX #1570: Enhance the test coverage of fixedRate controller.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                FIX #1570 
## Checklist
 - [X]  A link to the issue/user story that the pull request relates to

## Existing issues
No

## Automated Tests
Enhance the tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 13:40:32 +0000 UTC
    </div>
</div>

