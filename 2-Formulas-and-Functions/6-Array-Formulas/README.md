What I Learned
-
I learned how Excel arrays allow formulas to operate on entire ranges at once, enabling row-by-row calculations without helper columns.

Key Concepts
--
An array is a collection of values processed simultaneously.

Logical tests on ranges return TRUE/FALSE arrays, which Excel evaluates element-by-element.

Arithmetic operators (*, +) convert logic into numeric filters (1/0).

Practical Skills
-
Applied multiple conditions to ranges using array logic.

Replaced AND() / OR() with mathematical operators for correct row-level evaluation.

Used SUMPRODUCT to perform conditional calculations without Ctrl+Shift+Enter.

Computed sum, count, average, and median from filtered datasets.

Handled large datasets efficiently (30k+ rows).

Example
=SUMPRODUCT((A2:A1000="AA")*(M2:M1000))


Filters rows where A = "AA" and sums the corresponding values in column M.

Outcome
-
Enabled cleaner formulas, fewer helper columns, and more scalable data analysis in Excel.
