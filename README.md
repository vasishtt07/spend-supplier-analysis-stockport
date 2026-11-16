# Spend & Supplier Analysis: Stockport Council purchase orders

A practice spend analysis on public-sector purchase-order data: where the money goes, how concentrated it is across suppliers, and where a procurement team could save. This is an independent analysis of public data, not client work.

**Files**
- `Spend_Supplier_Analysis_Deck.pdf`: the 6-slide recommendation deck.
- `Stockport_Spend_Analysis.xlsx`: the workbook behind it (Category_Summary, Supplier_Pareto with chart, Tail_Spend, Savings_Model with editable assumptions, Clean_Data with every line and its exclusion flag).

## Key findings
- 2,185 purchase-order lines over £5,000, £160.1M in total, across four quarters.
- £78.7M (49%) is treated as non-addressable (NHS bodies, other councils, council-linked companies, and the Healthcare, Fees and Charges and Utilities categories), leaving £81.4M across 544 suppliers.
- 11 suppliers (2%) carry 50% of addressable spend, and 55 (10%) carry 80%.
- 395 suppliers (72.6%) have under £50k of spend each. Together they account for £6.7M (8.2%).
- Consultancy is the most fragmented category: 131 suppliers, 100 of them tail.
- Illustrative savings of £1.4M to £5.0M (1.8% to 6.1% of addressable spend) across six categories, with a base case of about £3.2M (3.9%).

## Method
1. Combined four quarterly purchase-order files and standardised supplier names (case, punctuation, Ltd/Limited/PLC).
2. Used the council's own product-class description as the spend category.
3. Flagged non-addressable lines, then built a spend cube by category and supplier.
4. Ranked suppliers by spend (Pareto) and counted tail suppliers (under £50k) overall and per category.
5. Sized savings levers per category with low, base and high percentages.

## Assumptions and limits
- The data covers purchase-order lines over £5,000 only, and the four quarters are not consecutive (Jul–Sep 2023, Oct–Dec 2023, Jan–Mar 2024, Apr–Jun 2025). The totals are not annual spend.
- The non-addressable list is a judgement call. Each line is flagged in `Clean_Data` so it can be changed.
- The savings percentages are illustrative assumptions, not benchmarks. They are the yellow cells in `Savings_Model` and the totals update when they change.

## Data source and licence
Stockport Council, "Purchase orders over £5,000", published on data.gov.uk. Contains public sector information licensed under the Open Government Licence v3.0.

Author: Vasishtt S G
