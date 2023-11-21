---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    Secret Keeper Application
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **What this PR does / why we need it**:

Create a new demo application ~ Secret Keeper

Secret Keeper has 5 functions.
InitSecretKeeper:
- This function will initialize the key "AUTH_LIST_KEY" with value ["Alice", "Bob"] and key "SECRET_KEY" with value "DefaultSecret".
- This function should only be called once when the application started.
- Of course a malicious user can call this function to reset the value, but this we will assume this is not what an attacker would want to achieve. RevealSecret:
- This function allow users that in the Authlist ("AUTH_LIST_KEY") able to reveal the value of secret stored under key "SECRET_KEY". LockSecret:
- This function allow users that in the Authlist ("AUTH_LIST_KEY") able to store a new value of secret under key "SECRET_KEY".
- The old value will be replaced. AddUser:
- This function allow users that in the Authlist ("AUTH_LIST_KEY") able to add a new user to the Authlist.
- Then the new user can now perform the following four functions (RevealSecret, LockSecret, AddUser, RemoveUser) RemoveUser:
- This function allow users that in the Authlist ("AUTH_LIST_KEY") able to add remove an existing user off the Authlist.
- Then the removed user can no longer able to perform the following four functions (RevealSecret, LockSecret, AddUser, RemoveUser)

Example using fpc-simple-client:
./fpcclient invoke initSecretKeeper
./fpcclient query revealSecret Alice
./fpcclient invoke lockSecret Bob NewSecret
./fpcclient query revealSecret Alice
./fpcclient invoke removeUser Alice Bob
./fpcclient query revealSecret Alice
./fpcclient query revealSecret Bob  // (will failed) ./fpcclient invoke addUser Alice Bob
./fpcclient query revealSecret Bob // (will success)


**Which issue(s) this PR fixes**:

This is just create a new application for ppc example

**Special notes for your reviewer**:



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 15:21:58 +0000 UTC
    </div>
</div>

