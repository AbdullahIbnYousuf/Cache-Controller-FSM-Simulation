# Report Outline

This file is a structure/checklist only. Write the final report in your own words.

## 1. Cover Page

- Assignment title
- Course name/code
- Student name(s)
- Student ID(s)
- Submission date

## 2. Introduction

- Goal of the project
- Why FSM is suitable for cache controller logic
- Scope and assumptions (simple CPU queue, memory fixed latency)

## 3. Simulator Setup

- Language and tools used
- Project structure overview
- Build and run steps
- Input workload format

## 4. Cache Controller FSM Design

- Policies used: direct-mapped, write-back, write-allocate
- State list and transitions
- Signal responsibilities in each major state
- Include FSM flowchart/diagram

## 5. Experimental Workloads

Use at least 3 workloads:

- Full functionality workload
- Hit-focused workload
- Writeback-focused workload

For each workload include:

- Input sequence
- Key cycle trace rows
- Summary counters (hits, misses, writebacks)
- Interpretation of behavior

## 6. Detailed Signal Analysis

Discuss behavior of:

- `cpu_req_ready`, `cpu_stall`
- `cache_hit`, `cache_miss`
- `mem_rd`, `mem_wr`, `mem_ready`, `mem_data_valid`
- `data_out_valid`, `data_out`

## 7. Validation Against FSM Idea

- Show that implemented transitions match your FSM diagram
- Mention how writeback and allocation phases maintain correctness

## 8. Limitations and Future Work

Example points:

- Single-word line model
- Blocking cache only
- No replacement policy beyond direct mapping
- Could be extended to set-associative or non-blocking behavior

## 9. Conclusion

- What you achieved
- Key learning outcomes

## 10. Appendix (Optional)

- Selected code snippets
- Additional trace excerpts
- GitHub repository link
