# Association Rule Learning Metrics

Support, Confidence, and Lift are used to measure how useful and meaningful an association rule is.

## Support

Support tells us how often a rule appears in the entire dataset.

### Example

Rule:

```text
Milk -> Bread
```

If there are 100 transactions and both Milk and Bread appear together in 25 transactions:

```text
Support = 25 / 100 = 0.25
```

### Simple Meaning

> How common is this rule?

---

## Confidence

Confidence tells us how often the rule is correct.

### Example

Rule:

```text
Milk -> Bread
```

If Milk appears in 40 transactions and Milk + Bread appear together in 30 transactions:

```text
Confidence = 30 / 40 = 0.75
```

### Simple Meaning

> If a customer buys Milk, how often do they also buy Bread?

---

## Lift

Lift tells us how much stronger the rule is compared to random chance.

### Example

Rule:

```text
Milk -> Bread
```

Suppose:

```text
Confidence = 0.75
Support(Bread) = 0.25
```

Then:

```text
Lift = 0.75 / 0.25 = 3
```

### Simple Meaning

> Is this relationship actually interesting, or would it happen anyway?

### Interpretation

```text
Lift = 1  -> No relationship

Lift > 1  -> Positive relationship

Lift < 1  -> Negative relationship
```

Higher Lift means a stronger association.

---

## Quick Summary

| Metric     | Meaning                                           |
| ---------- | ------------------------------------------------- |
| Support    | How common is the rule?                           |
| Confidence | How often is the rule correct?                    |
| Lift       | How much stronger is the rule than random chance? |
