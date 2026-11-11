---
name: cogs-calculator
displayName: COGS calculator
description: >-
  Calculate cost of goods sold from beginning inventory, period purchases, and
  ending inventory. Use to reconcile stock costs, calculate gross profit and
  margin from matching revenue, or compare inventory scenarios.
---

# COGS calculator

Use the [COGS calculator](https://doany.ai/tools/cogs-calculator?utm_source=skills.sh&utm_medium=skill&utm_campaign=cogs-calculator&utm_content=cogs-calculator) to check the inventory roll-forward and download the reconciliation.

## Gather values on one basis

Get opening and closing inventory values at cost and purchases for the same period and currency. Confirm which purchase costs are included. If the user wants gross profit, get net sales revenue on the same period and product scope. Use the user's accounting valuation basis for inventory.

## Reconcile the roll-forward

1. Add beginning inventory and purchases to find goods available at cost. Subtract ending inventory to obtain COGS.
2. If ending inventory exceeds the cost pool, flag the discrepancy and ask about transfers, adjustments, or omitted purchases before presenting it as ordinary COGS.
3. If revenue is supplied, calculate gross profit as revenue less COGS. Divide gross profit by positive revenue for gross margin. State that the result covers inventory and sales and list any operating expenses outside the inputs.
4. Return the opening value, purchases, ending value, COGS, and optional gross profit and margin. A comparison must keep inventory valuation consistent across scenarios.

## Browser workflow

When the page exposes browser actions, use `calculate_cogs` and `get_cogs` to verify the inventory figures and any optional gross profit and margin before exporting.

## Example

Beginning inventory of $5,000 plus $7,000 in purchases less $4,500 ending inventory gives $7,500 COGS. With $12,000 in matching revenue, gross profit is $4,500 and gross margin is 37.5%.
