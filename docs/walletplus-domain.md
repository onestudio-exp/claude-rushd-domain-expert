# WalletPlus Domain Knowledge

## Product Overview
WalletPlus is a Salla app designed to increase repeat purchases, customer retention, and referrals through wallet-based rewards and cashback systems.

---

## Core Entities

- Merchant
- Customer
- Order
- Order Status
- Wallet
- Cashback Rule
- Referral Program
- Referral Relationship
- Reward Transaction

---

## Core Workflows

### 1. Cashback Flow
Order → validation → completion → reward calculation → wallet credit

### 2. Referral Flow
Referral link → customer signup → order → validation → commission allocation

### 3. Wallet Flow
Balance → earn → redeem → update → audit

---

## Business Rules

- Rewards are ONLY issued after order completion
- Canceled or returned orders invalidate rewards
- No self-referrals allowed
- Cashback can be restricted by product or category
- Wallet balance must always be consistent and auditable

---

## Domain Complexity

The system is NOT simple CRUD.

It involves:
- Order lifecycle handling
- Fraud prevention
- Reward timing logic
- Wallet accuracy
- Interaction between cashback and referral systems

---

## Common Risks

- Issuing rewards before order completion
- Fraud through duplicate accounts
- Incorrect reward calculation
- Wallet inconsistencies

---

## Anti-Patterns

- Reward on order creation
- Mixing cashback and referral logic
- No transaction history
- Business logic in frontend
