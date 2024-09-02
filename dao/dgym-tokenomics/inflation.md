---
icon: money-bill-trend-up
description: This section contains everything about the DGYM inflation
---

# Inflation

Stakeholders can stake their DGYM tokens to earn rewards. The reward distribution is based on the amount staked and the duration for which the tokens are staked. The longer the tokens are staked, the higher the reward. These rewards are generated through the inflation explained in this document.

## <mark style="color:green;">DGYM Token Inflation Mechanism</mark>

The DGYM Token employs an inflation mechanism **designed to regulate the token supply dynamically**. This document explains how the inflation mechanism works and provides details about the smart contract's behavior.

### Parameters

* **Inflation Decay Constant**: 0.046% (Approx 17% annual decay)
* **Max Supply**: 10,000,000,000 DGYM
* **Initial Supply**: 1,000,000,000 DGYM
* **Inflation Interval**: Daily



{% hint style="info" %}
These parameters can be modified through the DAO voting&#x20;
{% endhint %}

### Inflation Rate Calculation

The daily inflation rate is dynamically calculated based on the remaining supply ratio and a decay constant. The formula used is:

$$
Y_c = D_c \times \left( \frac{S_m - S_c}{S_m} \right)
$$





Where:

* $$D_c$$ is the inflation decay constant (daily).
* $$S_m$$ is the maximum supply.
* $$S_c$$ is the current supply.

### Inflation Application

The inflation is applied daily. When the inflation is applied, new tokens are minted and added to the total supply. **The total supply asymptotically approaches the the max supply**.



<figure><img src="../../.gitbook/assets/temp (1).jpg" alt=""><figcaption><p>Total Supply and Inflation Rate Over Time</p></figcaption></figure>

## <mark style="color:green;">**Impact of Inflation on the Economy**</mark> <a href="#impact-of-inflation-on-the-economy" id="impact-of-inflation-on-the-economy"></a>

The DeGym's inflation model is meticulously designed to balance new token creation with economic incentives for stakeholders. By adjusting block rewards and modeling inflation rates, DeGym aims to encourage network security and participation while gradually transitioning to a more stable token economy. This approach not only secures the network but also aims at a fair distribution of rewards, thereby ensuring the long-term viability and value of the DGYM token.

DeGym's innovative approach to managing inflation through its tokenomics and reward systems demonstrates a sophisticated understanding of DAO economy dynamics. The daily reduction in rewards and carefully calibrated inflation rate are central to DeGym's strategy for creating a stable and sustainable economic model that benefits stakeholders and the broader ecosystem.&#x20;

The DGYM Token's inflation mechanism ensures that the token supply is dynamically regulated while rewarding stakeholders based on their contribution and commitment. The smart contract implementation **ensures fairness and transparency** in the distribution of rewards.
