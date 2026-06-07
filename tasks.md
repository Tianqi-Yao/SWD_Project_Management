# Research Tasks & Timeline

> Status: `Todo` / `In Progress` / `Done`
> Priority: `High` / `Medium` / `Low`
>
> **`#` column:** GitHub issue number for reference and linking.
> **`ID` column:** Custom hierarchical ID — `Px-NN` for main issues, `Px-NN-NN` for sub-issues.
>
> | Symbol  | Meaning                                                     |
> |---------|-------------------------------------------------------------|
> | `#19`   | Main GitHub Issue                                           |
> | `↳ #43` | GitHub Sub-issue (own number, tracked on board)             |
> | `↳`     | Checkbox only (in parent issue body, not a separate issue)  |
> | `new`   | Pending — Claude creates on sync and backfills `#` and `ID` |
> | `↳ new` | Pending Sub-issue — same as above                           |
>
> Deps: issue numbers this task waits on, e.g. `#19` or `#19 #20`. Leave blank if none.

---

## P1 · SWD Vision

### Milestone 1 — Data & Model Foundation

| #     | ID       | Title                                                                   | Status      | Priority | Start      | End        | Deps |
|-------|----------|-------------------------------------------------------------------------|-------------|----------|------------|------------|------|
| #19   | P1-01    | 64MP Dataset Annotation                                                 | Done        | High     | 2026-05-27 | 2026-06-05 |      |
| ↳ #43 | P1-01-01 | Rounds 1 & 2: annotation batches                                        | Done        | High     | 2026-05-27 | 2026-05-29 |      |
| ↳ #44 | P1-01-02 | Round 3: 3rd annotation batch                                           | Done        | High     | 2026-06-01 | 2026-06-05 |      |
| #37   | P1-02    | Mid-Missouri Data Collection                                            | In Progress | High     | 2026-05-27 | 2026-10-31 |      |
| ↳ #45 | P1-02-01 | Round 1: Mid-Missouri farm collection (Airport, Jefferson City)         | Done        | High     | 2026-06-02 | 2026-06-02 |      |
| ↳ #46 | P1-02-02 | Round 2: Mid-Missouri farm collection (Airport, Jefferson City)         | Todo        | High     | 2026-06-08 | 2026-06-08 |      |
| #54   | P1-03    | South Missouri Data Collection                                          | In Progress | High     | 2026-05-27 | 2026-10-31 |      |
| ↳ #55 | P1-03-01 | Round 1: South Missouri farm collection                                 | Todo        | High     | 2026-06-10 | 2026-06-10 |      |

### Milestone 2 — Models

| #     | ID       | Title                                            | Status      | Priority | Start      | End        | Deps |
|-------|----------|--------------------------------------------------|-------------|----------|------------|------------|------|
| #21   | P1-04    | 64MP Camera Insect Detection Model Pipeline      | In Progress | Medium   | 2026-05-30 | 2026-06-30 |      |
| ↳ #48 | P1-04-01 | Round 2: instance segmentation model — 32 images | Done        | Medium   | 2026-05-30 | 2026-05-31 | #19  |
| ↳ #49 | P1-04-02 | Round 3: instance segmentation model — xx images | Todo        | Medium   | 2026-06-06 | 2026-06-07 | #19  |
| #38   | P1-05    | 64MP Camera Insect Classification Model Pipeline | In Progress | Medium   | 2026-06-13 | 2026-06-14 |      |
| ↳ #50 | P1-05-01 | Round 1: classification model — xx images        | Todo        | Medium   | 2026-06-13 | 2026-06-14 | #21  |
| #39   | P1-06    | 64MP Camera SWD Detection Model Pipeline         | In Progress | Medium   | 2026-06-20 | 2026-06-21 |      |
| ↳ #51 | P1-06-01 | Round 1: SWD detection model — xx images         | Todo        | Medium   | 2026-06-20 | 2026-06-21 | #38  |
| #22   | P1-07    | (option) Insect Body Part Semantic Segmentation  | Todo        | Low      | 2026-06-21 | 2026-06-22 | #39  |

### Milestone 3 — Evaluation

| #   | ID    | Title                            | Status | Priority | Start | End | Deps |
|-----|-------|----------------------------------|--------|----------|-------|-----|------|
| #20 | P1-08 | 64MP vs 16MP Baseline Comparison | Todo   | Medium   | 2026-08-01 | 2026-10-31 | #39  |

---

## P2 · IoT Paper

### Field Deployment

| #   | ID    | Title                                                                               | Status      | Priority | Start      | End        | Deps |
|-----|-------|-------------------------------------------------------------------------------------|-------------|----------|------------|------------|------|
| #40 | P2-01 | Complete Latest SmartTrap Design                                                    | Done        | High     | 2026-05-15 | 2026-06-07 |      |
| #41 | P2-02 | Design and Test Rpi Power Monitoring Module                                         | In Progress | High     | 2026-05-27 | 2026-06-07 |      |
| #24 | P2-03 | Sanborn Field & Airport Field Deployment (3+4 Devices — Network & Power Monitoring) | Todo        | High     | 2026-06-12 | 2026-06-30 | #41  |

### Data Collection & Writing

| #   | ID    | Title                                                             | Status | Priority | Start      | End        | Deps    |
|-----|-------|-------------------------------------------------------------------|--------|----------|------------|------------|---------|
| #26 | P2-04 | Data Collection: Power / Network / Environmental / System Metrics | Todo   | High     | 2026-05-15 | 2026-07-30 | #24 #20 |
| #27 | P2-05 | Write IoT System Evaluation Paper                                 | Todo   | High     | 2026-09-01 | 2026-08-15 | #26     |

---

## P3 · Prediction

| #   | ID    | Title                                                                 | Status | Priority | Start      | End        | Deps |
|-----|-------|-----------------------------------------------------------------------|--------|----------|------------|------------|------|
| #28 | P3-01 | Organize Data (SWD Counts + Temp/Humidity from Field and Our Sensors) | Todo   | Low      | 2026-06-15 | 2026-06-30 | #20  |

---

## P4 · Farm-NG The Amiga

### Exploration

| #   | ID    | Title                              | Status | Priority | Start      | End        | Deps |
|-----|-------|------------------------------------|--------|----------|------------|------------|------|
| #42 | P4-01 | Rebuild Amiga Platform Form Factor | Todo   | Low      | 2026-06-08 | 2026-06-10 |      |
| #29 | P4-02 | Obstacle Detection Exploration     | Todo   | Low      | 2026-06-15 | 2026-06-30 |      |
| #30 | P4-03 | Vision Navigation Exploration      | Todo   | Low      | 2026-06-15 | 2027-06-30 | #29  |

---

## P5 · 3DGS

### Pipeline

| #   | ID    | Title                    | Status | Priority | Start      | End        | Deps |
|-----|-------|--------------------------|--------|----------|------------|------------|------|
| #31 | P5-01 | Nerfstudio Workflow Setup | Todo   | Medium   | 2026-06-15 | 2026-06-30 |      |
| #32 | P5-02 | 3DGS Data Collection     | Todo   | Medium   | 2026-06-15 | 2026-06-30 | #31  |

---

## P6 · Corn Leafhopper

### Evaluation Series

| #   | ID    | Title                                                        | Status | Priority | Start      | End        | Deps |
|-----|-------|--------------------------------------------------------------|--------|----------|------------|------------|------|
| #33 | P6-01 | Rpi Dual-Camera Simultaneous Operation Feasibility Test      | Todo   | Medium   | 2026-06-01 | 2026-06-07 |      |
| #34 | P6-02 | Optimal Installation Distance Test                           | Todo   | Medium   | 2026-06-07 | 2026-06-08 | #33  |
