---
description: A collectively-owned organization working towards a shared mission.
---

# 👥 Organization

DAO is self-governing organization that operate on smart contracts, allowing for transparent decision-making and governance.

Starting an organization with someone that involves funding and money requires a lot of trust in the people you're working with. But it’s hard to trust someone you’ve only ever interacted with on the internet. With DAOs we don’t need to trust anyone else in the group, just the DAO’s code, which is 100% transparent and verifiable by anyone.

The DAO allow us to work with like-minded folks around the globe without trusting a benevolent leader to manage the funds or operations. There is no CEO who can spend funds on a whim or CFO who can manipulate the books. Instead, blockchain-based rules baked into the code define how the organization works and how funds are spent.

This opens up so many new opportunities for global collaboration and coordination. **DeGym is managed by the DeGym DAO**. The DAO members govern DeGym to ensure its efficiency and stability. The DeGym DAO should do the following

## Scope & Functions <a href="#scope-of-the-dao" id="scope-of-the-dao"></a>

The DeGym DAO have built-in treasury that no one has the authority to access without the approval of the group. The DeGym DAO should do the following:

* Build, deploy, update, and decide on key parameters of staking protocols, approve incentives for parties that contribute towards DAO’s goals;
* Approve DGC (DeGym Grant Committee) grants to support different research and initiatives that are worked upon for the benefit of the protocol;
* Payments to full-time contributors and other operational duties;
* Bug bounty program, respond to emergencies;
* Accumulation of service fees from DeGym, which can be funneled into the insurance and development funds, distributed by the DAO;

Decisions are governed by proposals and voting through the voting power of governance token (`DGYM`) to ensure everyone in the organization has a voice, and everything happens transparently on-chain. It manages the degym protocol and all possible future sub-protocols by deciding on key parameters:

* Inflation Decay Constant
* Max Supply
* Staking epoch lengths
* Oracles

The DAO is the logical compromise between a team or a community-driven protocol, which allows the deployment of competitive products without full centralization and custody of the exchanges.

## **Council**

For the DeGym network to remain healthy and viable in the long-term, it must be adaptable and responsive to the network stakeholders’ demands over time. To that end we propose the following governance model, and welcome feedback from the broader community. For the avoidance of doubt, the right to vote does not entitle DeGym token holders to vote on the operation and management of the Foundation, its affiliates, or their assets, and does not constitute any equity interest in any of these entities.

Since voter turnout is a persistent problem in almost all electoral systems – including decentralized ecosystems – a council will be elected to represent the interests of passive stakeholders in the DeGym network. These Council Members may determine features and/or parameters of DeGym as well as protocol improvements and new product development, or even changes to the governance process itself.

The size of the council will increase as the network size increases. The size of the council will be determined at network launch, starting with a relatively smaller number and then scaling upward as the network matures.

### **Purview**

The council will vote on decisions that impact all aspects of the DeGym network, including anything from code upgrades to adjustments to the reward mechanism. These changes will eventually be encoded into each node’s codebase that will automatically enact approved decisions.

### **Election**

The council will be elected via a single transferable vote (STV) system, with the number of votes determined by the number of DeGym tokens held by each voter with a bonding time modifier (see below). This is a widely used voting system to achieve proportional representation through ranked voting for multi-seat organizations. Here’s a simple description of the STV system with a Droop quota.

_Premises_

* N seats are available
* V valid votes are cast
* T is the minimum threshold of votes necessary to win any given seat, with T = ceil (valid votes cast / (seats to fill + 1))

_Voting steps_

1. Council candidates nominate themselves
2. Stakeholders cast their votes for their most preferred N candidates ranking from most to least preferred
3. Starting from all stakeholders’ first choice votes
4. Any candidate receiving votes greater than T is elected into the council
5. The elected candidates’ received votes in excess of T are transferred to those voter’s next choice
6. If no candidate receives votes in excess of T, eliminate the candidate with the least number of votes and transfer those votes to the voter’s next preferred candidate
7. Repeat steps 4-6 until we have either elected a candidate for every seat, or the number of remaining seats equal to the number of remaining candidates – in which case those remaining candidates are elected

**Council Member Terms**

Each council member has a term of approximately 12 weeks. In actual implementation, the term will be determined by counting the number of periods that have elapsed. As the network grows and council expands, we will try to stagger the terms to make sure only a portion of the council members are up for reelection at any given election cycle.

***

Preparation for governance votes & communication will be managed via Dedicated [Discord](https://discord.gg/zFSBQtfF) channels. Voting will be conducted via Snapshot.
