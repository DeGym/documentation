---
icon: function
description: >-
  This document provides a detailed explanation of how the voucher's price
  calculation work
---

# Pricing

The DeGym NFT-based voucher pricing function is designed to calculate the price of a voucher based on two primary factors: **tier** and **durability**. The pricing model also includes a decay factor, which adjusts the price over time to ensure fairness and incentivize early purchases. The pricing model rewards users who opt for longer durations, offering better value as the duration increases.

## <mark style="color:green;">System Parameters</mark>

The following parameters are internal voucher parameters in the respective of a given ERC20 token  determined by the DAO (commercial tokens), which can be changed anytime by voting mechanism:

* $$B_P$$: BASIC\_PRICE — the base price for a 1-month.
* $$M_P$$: MIN\_BASE\_PRICE\_FACTOR — the factor determining the minimum allowable base price.
* $$D_R$$: DECAY\_RATE — the rate at which the base price decreases as the duration increases.

## <mark style="color:green;">**Function**</mark>

The pricing of a voucher is determined by the following formula:

$$
Price=max(B_P​×(1−D_R​×(\frac{30}{D}​−1)),M_P​×B_P​)×T×\frac{30}{D​}
$$

Where:

* $$T$$:  tier — the tier level of the voucher, which acts as a multiplier.
* $$D$$:  duration — the duration of the voucher in days.

This formula calculates the voucher price by:

1. Adjusting the base price based on the duration. The longer the duration, the more favorable the pricing.
2. Ensuring that the price does not fall below a certain threshold, which is determined by the minimum base price factor.
3. Multiplying by the tier and the normalized duration to arrive at the final price.

