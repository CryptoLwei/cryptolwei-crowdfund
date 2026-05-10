# 🚀 CrowdFund — ERC-20 Crowdfunding on Ethereum

Decentralized crowdfunding using ERC-20 tokens. Goals met = creator claims. Goals missed = contributors refunded. Built on HackQuest.

## What It Does
- Launch campaigns with a goal, start, and end time
- Pledge / unpledge ERC-20 tokens during active window
- Creator claims if goal is met
- Automatic refunds if goal is missed
- MockToken (MCK) included for testing

## Functions
| Function | Description |
|----------|-------------|
| `launch(goal, startAt, endAt)` | Create a campaign |
| `pledge(id, amount)` | Fund a campaign |
| `unpledge(id, amount)` | Withdraw your pledge |
| `claim(id)` | Creator claims if goal met |
| `refund(id)` | Reclaim tokens if goal missed |

## Tech Stack
- Solidity `^0.8.24` · ERC-20 · Ethereum · HackQuest

## Deploy & Test
1. Deploy `MockToken` → copy address
2. Deploy `CrowdFund(mockTokenAddress)`
3. Launch campaign → approve → pledge → claim or refund
