# Before vs After — Domain Expert Impact

## Test Task
"Add cashback immediately after order creation to improve user experience."

---

## ❌ Without Domain Expert

- AI implemented cashback on order creation
- Ignored order status lifecycle
- No validation for refunds or returns
- No fraud detection
- Wallet updated instantly
- No audit or rollback logic
- Business logic placed in frontend
- UX was misleading (user sees rewards that may disappear)

---

## ⚠️ Issues

- High fraud risk
- Incorrect rewards
- Merchant financial loss
- Broken trust
- System inconsistency

---

## ✅ With Domain Expert (Rushd)

### Decision:
❌ Reject the request

### Why:
Cashback must only be issued after order completion to ensure transaction validity.

### Risks:
- Refund exploitation
- Fake orders
- Wallet abuse

### Safer Alternative:
- Show "Pending Cashback" to the user
- Release reward only after order completion

### Impact:
- Protects merchants
- Prevents fraud
- Maintains system integrity
- Improves user trust

---

## 🧠 Key Insight

The domain expert did NOT improve the code.

It improved the thinking.

It transformed AI from:
→ Answering

Into:
→ Decision-making
