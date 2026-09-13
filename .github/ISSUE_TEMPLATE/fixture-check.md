---
name: Fixture check
about: Ask the pipeline to look at one upcoming Premier League fixture
title: "Fixture check: "
labels: request
---

Fill in the fields below. Everything else on this page is ignored.

fixture:
kickoff_utc:
requested_by: owner
request_type: fixture_check
note:

<!--
requested_by must be owner. The analysts may not file requests: an analyst
asking the pipeline to look at something would blur a request with a
selection.

A request asks the pipeline to research a fixture. It carries no selection,
no stake and no authority to bet, it cannot alter the ledger, and it cannot
skip a methodology gate. Fields such as selection, stake_gbp, or price are
refused outright rather than stored -- a request asks for research, it does
not set the outcome.
-->
