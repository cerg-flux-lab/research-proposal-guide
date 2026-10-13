# Gantt chart template

Mermaid renders natively on GitHub. Replace the dates and tasks. One section per objective; writing runs in parallel; include fixed institutional dates.

Do not use a colon in a task name. Mermaid splits each task line at the first colon, so `Deliverable: report :milestone, ...` is a syntax error. Colons are fine in the chart title and in section names.

```mermaid
gantt
    title Research plan: [working title]
    dateFormat  YYYY-MM
    axisFormat  %b %y

    section Proposal
    Literature review and concept note      :done,    p1, 2027-02, 2027-04
    Proposal writing                        :active,  p2, 2027-04, 2027-06
    Proposal defence                        :milestone, m1, 2027-06, 0d

    section Objective 1: verified solver
    Implement core solver                   :o1a, 2027-06, 2027-09
    Code verification (analytical cases)    :o1b, 2027-08, 2027-10
    Solution verification (convergence)     :o1c, 2027-10, 2027-11
    Verification report delivered           :milestone, m2, 2027-11, 0d

    section Objective 2: validation
    Validation case setup                   :o2a, 2027-11, 2028-01
    Validation runs and comparison          :o2b, 2028-01, 2028-04
    Conference paper submission             :milestone, m3, 2028-04, 0d

    section Objective 3: parametric study
    Test matrix execution                   :o3a, 2028-04, 2028-09
    Analysis and uncertainty quantification :o3b, 2028-08, 2028-10

    section Writing
    Chapters 1 and 2 (background, literature)  :w1, 2027-07, 2027-12
    Chapter 3 (method)                         :w2, 2027-12, 2028-03
    Chapters 4 and 5 (results, discussion)     :w3, 2028-05, 2028-11
    Journal paper                              :w4, 2028-09, 2029-01
    Full draft to supervisor                   :milestone, m4, 2028-12, 0d
    Revision and submission                    :w5, 2029-01, 2029-03

    section Institutional
    Annual progress report                  :milestone, i1, 2028-02, 0d
    Contingency                             :crit, c1, 2029-03, 2029-05
```

## Typical durations

| Phase | MEng (2 years) | PhD (3 to 4 years) |
|---|---|---|
| Proposal | 3 to 4 months | 4 to 6 months |
| Method development and verification | 5 to 6 months | 9 to 12 months |
| Validation and main study | 6 to 8 months | 12 to 18 months |
| Writing (overlapping) | from month 6 | from month 9 |
| Contingency | 2 months | 3 to 4 months |

Check your Department's minimum and maximum registration periods and the examination submission windows; they fix the end date, so plan backwards from it.
