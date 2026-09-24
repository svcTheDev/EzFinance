# Requirements Document

Project name:
EzFinance

Problem statement:

The user has to download different bank trasactions distributed across different financial institutions normalize and categorize the data, and manually create an analysis to understand their expeses and get an overview of their finances

Primary users:
- Me (referred as user in this document)

Functional requirements:

REQ-F-001
The user must be able to upload a supported XLSX bank statement.

REQ-F-002
The system must display a review step before confirming an import.

REQ-F-003
The import review must display the uploaded filename and the number
of transaction rows detected.

REQ-F-004
The import review must display how source columns are mapped
to ezFinance transaction fields.

REQ-F-005
The user must be able to confirm or cancel a reviewed import.

REQ-F-006
The user must be able to view imported transactions in a table.

REQ-F-007
The user must be able to edit permitted transaction fields inline
from the Transactions screen.

REQ-F-008
Changes made to a transaction must immediately affect the
corresponding financial calculations.

REQ-F-009
The user must be able to filter dashboard information by month
or full year.

REQ-F-010
Only months and years containing transaction data must be selectable.

REQ-F-011
The dashboard must display total income, mandatory expenses,
voluntary expenses and balance for the selected period.

REQ-F-012
The dashboard must display a breakdown comparing income
and total expenses for the selected period.

REQ-F-013
The dashboard must display financial records including highest income,
highest voluntary expense, highest mandatory expense and highest
saved amount.

REQ-F-014
When no transaction history exists, the dashboard must display
an empty state that directs the user to import a statement.


Non-functional requirements:

REQ-NF-001: A supported statement containing up to [X] transactions must be
processed and displayed within [Y] seconds under normal conditions.
REQ-NF-002: From the main import screen, the user must be able to select and submit a bank statement in no more than two user actions.
REQ-NF-003: User only interaction should be just to categorize transactions manually for the first time

Business rules:
BR-001: Re-importing the same statement does not create duplicate transactions.
BR-002: Only statements from supported financial institutions and supported file formats may be imported.
BR-003: Every successfully imported transaction must be classified as either income or expense before it contributes to financial totals.
BR-004: A transaction may have only one active category at a time.
BR-005: Changing a transaction category must not create a new transaction or modify its financial amount.
BR-006: Transactions that cannot be normalized safely must not silently enter financial calculations as valid transactions.
BR-007: The dashboard must calculate financial totals only from successfully imported and normalized transactions.
BR-008: Invalid trasactions identified in the files will be tag as "uncategorized" and won't count for the final overview

System constraints:
CON-001: [Technology, budget, time, environment, or integration limit].
Acceptance criteria:
AC-001:
Given [starting condition],
When [action happens],
Then [expected result].
Open questions:
- [Anything that must be clarified before design or coding begins]