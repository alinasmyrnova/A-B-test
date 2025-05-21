# A/B Testing Analysis of New Search Ranking Algorithm

## Project Overview

The purpose of this experiment is to evaluate the impact of a new search ranking algorithm designed to improve booking conversion rates for an online travel agency. The Product team wants to ensure the new algorithm delivers a statistically significant uplift in conversion without negatively impacting the booking speed.

Primary Objective:
Improve the booking conversion rate (percentage of sessions resulting in a booking).

This project involves analyzing experimental data from an A/B test, comparing a control group (existing ranking) to a variant group (new ranking), and making a data-driven recommendation for rollout.

---

## Data

- **sessions_data.csv**: Session-level data including session IDs, user IDs, session start time, booking timestamps, and time to booking.
- **users_data.csv**: User-level data with logged-in users and their assignment to control or variant groups.

---

## Objectives

- Prepare and merge datasets properly, ensuring only logged-in users are included.
- Create a primary metric — session-level conversion (booking or no booking).
- Conduct sanity checks (Sample Ratio Mismatch test) to validate randomization.
- Analyze the primary metric (conversion) for statistically significant uplift using Z-test.
- Analyze guardrail metric (time to booking) using t-test to ensure no negative impact.
- Calculate effect sizes to quantify improvements.
- Provide a clear recommendation to either fully roll out the new search ranking or pull back based on the experiment results.

---

## Tools & Methods

- Python (pandas, scipy)
- Statistical hypothesis testing (Z-test, t-test, Chi-square test)
- Effect size calculations
