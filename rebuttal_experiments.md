# Rebuttal Experiments

---

**Table 1 Caption**:Performance comparison of TimeSieve on the **UCI** **Retail** **dataset** with MAE as the evaluation metric. The results show the effect of different conditions: NP (No Perturbation), NPO (No Perturbation with Optimization), IP (Input Perturbation), and IPO (Input Perturbation with Optimization). For instance, at horizon 192, the model's error decreases from 0.461 (IP) to 0.381 (IPO). These results indicate that FTS consistently stabilizes predictions and improves overall accuracy in transactional data scenarios.  


|     | NP    | IP    | NPO   | IPO   |
| --- | ----- | ----- | ----- | ----- |
| 48  | 0.346 | 0.486 | 0.343 | 0.391 |
| 96  | 0.321 | 0.510 | 0.317 | 0.388 |
| 144 | 0.329 | 0.522 | 0.326 | 0.379 |
| 192 | 0.333 | 0.461 | 0.329 | 0.381 |


---

**Table 2 Caption**: MAE results of **TimeXer (ICLR 2024)** on the Wiki dataset under four conditions: NP (No Perturbation), IP (Input Perturbation), NPO (No Perturbation with Optimization), and IPO (Input Perturbation with Optimization). The results show that FTS consistently improves robustness across all horizons, reducing the performance drop caused by input noise—for example, at horizon 192, the error decreases from 0.445 (IP) to 0.331 (IPO).


|     | NP    | IP    | NPO   | IPO   |
| --- | ----- | ----- | ----- | ----- |
| 48  | 0.247 | 0.440 | 0.240 | 0.370 |
| 96  | 0.252 | 0.416 | 0.251 | 0.340 |
| 144 | 0.267 | 0.421 | 0.263 | 0.327 |
| 192 | 0.280 | 0.445 | 0.275 | 0.331 |


---

**Table 3 Caption**: MAE results of TimeSieve under the newly introduced **trend-based perturbation**. NP and IP refer to performance without and with perturbation (TS), while NPO and IPO include optimization (FTS). FTS effectively reduces the impact of trend drift—for example, at horizon 96, optimization lowers the error from 0.348 (IP) to 0.317 (IPO), demonstrating improved robustness under temporal shifts.


|     | NP    | IP    | NPO   | IPO   |
| --- | ----- | ----- | ----- | ----- |
| 48  | 0.381 | 0.421 | 0.377 | 0.406 |
| 96  | 0.309 | 0.348 | 0.303 | 0.317 |
| 144 | 0.320 | 0.349 | 0.315 | 0.333 |
| 192 | 0.319 | 0.377 | 0.318 | 0.358 |


---
**Table 4 Caption**: Evaluation on the ETTh1 dataset using **Quantile Loss (QL)** and **Wasserstein Distance (WD)** under different conditions. QL-NP and QL-NPO represent uncertainty estimation without and with optimization; WD-IP and WD-IPO measure distributional robustness under input perturbation. FTS consistently improves both metrics—for example, QL drops from 0.252 to 0.237 at horizon 192, and WD improves from 0.247 to 0.240 — demonstrating enhanced robustness across uncertainty and shift-aware evaluations.


|     | QL-NP | WD-IP | QL-NPO | WD-IPO |
| --- | ----- | ----- | ------ | ------ |
| 48  | 0.211 | 0.239 | 0.204  | 0.225  |
| 96  | 0.231 | 0.232 | 0.222  | 0.223  |
| 144 | 0.240 | 0.236 | 0.230  | 0.228  |
| 192 | 0.252 | 0.247 | 0.237  | 0.240  |


---

