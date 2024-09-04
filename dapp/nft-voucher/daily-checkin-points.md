---
icon: calendar-check
---

# Daily Checkin Points (DCP)

Daily Checkin Points (DCP) is a feature of the NFT-voucher system that rewards users for gym attendance and manages access based on NFT tiers.

## Overview

- DCP are granted when a customer buys or renews an NFT
- Points reset daily
- Both NFTs and gyms have tiers (1-99)
- DCP are consumed when checking in at a gym

## DCP Calculation

The amount of DCP granted daily is calculated as:

```
DCP = 2^(NFT_tier)
```


Where `NFT_tier` ranges from 1 to 99.

## Checkin Rules

1. **Gym Access Limit**: The number of times a user can access the same gym per day is equal to their NFT tier.
   - Example: Tier 1 NFT allows 1 visit, Tier 2 allows 2 visits, etc.

2. **DCP Consumption**: When checking in, the user consumes DCP based on the gym's tier:

   ```
   DCP_consumed = 2^(gym_tier)
   ```

3. **Checkin Requirement**: The user must have enough DCP to cover the gym's requirement.

## Examples

1. User with Tier 3 NFT:
   - Daily DCP: 2³ = 8 points
   - Can visit the same gym up to 3 times per day

2. Checking in at a Tier 2 gym:
   - DCP required: 2² = 4 points
   - User's remaining DCP after checkin: 8 - 4 = 4 points

3. Attempting to check in at a Tier 7 gym:
   - DCP required: 2⁷ = 128 points
   - Checkin fails (insufficient DCP)

## Implementation Considerations

- Reset DCP daily at a specific time (e.g., midnight)
- Track daily gym visits per user
- Implement DCP calculation and consumption logic
- Handle edge cases (e.g., insufficient DCP, exceeding daily gym limit)