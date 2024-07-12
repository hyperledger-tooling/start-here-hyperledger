---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/694" class=".btn">#694</a>
            </td>
            <td>
                <b>
                    first draft full repo readme via ai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Understanding the codebase for Carbon Sustain Integration

I'm currently working on understanding this codebase to explore integrating the CET system here with the enterprise carbon accounting, reduction, and offset product developed by [Carbon Sustain](https://socialimpact.linkedin.com/environmental-sustainability). We've also built a CET system on XRP and aim to connect these two systems using [Axelar](https://docs.axelar.dev/). [Once GMP calls are integrated](https://docs.axelar.dev/dev/general-message-passing/overview), the Carbon Sustain XRP CET system will be able to interact with the Solidity Smart Contracts in this repository to explore further integration possibilities.

However, navigating the codebase to understand its functionalities and how the different parts come together presents a significant challenge. There are many codebases, and it's unclear which readme to start with.

In an attempt to improve code comprehension, I've experimented with creating a consolidated README using an [AI tool](https://github.com/eli64s/readme-ai).

for the sake of reproducability, this is what i did:
1) install readmeai as written in their repo
2) run the following command:
```readmeai --repository https://github.com/hyperledger-labs/blockchain-carbon-accounting --api ollama --model mistral```
**note:** the model ran for 12 hours to complete.


My ultimate goal is to create verifiable emissions data systems that enable true carbon accounting and contribute to a greener society. This can be achieved by making this repository more approachable through initiatives like this one.

**Please note:** This is a first draft, and there might be errors due to limitations of the free [Mistral AI](https://mistral.ai/) model I used via [Ollama](https://ollama.com/) (4000 token character intake limit).

I'd appreciate your feedback on whether this is a worthwhile pursuit to continue.

Sincerely,
Kentaro
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-11 19:34:17 +0000 UTC
    </div>
</div>

