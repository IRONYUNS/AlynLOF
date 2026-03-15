# Adaptive Liza Yunus Nurzea Local Outlier Factor (AlynLOF)

## Abstract

This repository provides the implementation of **Adaptive Local Outlier Factor (AlynLOF)**, an anomaly detection algorithm that integrates the Granularity k-Nearest Neighbor (GkNN) method.

Unlike traditional LOF variants that require user-defined parameters, AlynLOF automatically determines an optimal neighborhood size by analyzing data granularity within the current streaming window. The algorithm maintains a constant-memory design using a fixed buffer of relevant data points and a weight-based mechanism (supported by a Kneedle-style strategy) to discard irrelevant instances, enabling scalable real-time anomaly detection.

The corresponding research article has been published in *Evolving Systems* (Springer).

> Basheer, M. Y. I., Ali, A. M., Hamid, N. H. A., Nordin, S., Osman, R., Yusoff, N., & Gu, X. (2026).  
> **Adaptive Local Outlier Factor.**  
> *Evolving Systems*, 17(2), 44.  
> https://doi.org/10.1007/s12530-026-09808-y

---

## Implementation Details

The algorithm is implemented in Python and was developed and executed using **Google Colab (cloud-based computational environment)**.

**Main file:**

```
AlynLOF.ipynb
```

The notebook can be directly uploaded and executed in Google Colab.

---

## Benchmark Datasets

We provide two available benchmark datasets:

1. **cardio.mat** — Cardiotocography dataset  
2. **glass.mat** — Glass identification dataset  

Both datasets are available from the **ODDS Library**:

S. Rayana, *ODDS Library*, 2016.  
http://odds.cs.stonybrook.edu/

The datasets are provided in `.mat` format and are widely used for anomaly detection benchmarking.

---

## Code Execution Instructions

To execute the code:

1. Open **Google Colab**.
2. Upload `AlynLOF.ipynb`.
3. Upload either `cardio.mat` or `glass.mat`.
4. Execute all cells sequentially.

---

## Dependencies

The implementation relies on the following Python libraries:

- numpy  
- scipy   
- pandas
- kneed
- scikit-learn
- h5py

Install dependencies (if running locally):

```bash
pip install numpy scipy pandas kneed scikit-learn h5py
```

---

## Citation

If you use this code in academic research, please cite:

Basheer, M. Y. I., Ali, A. M., Hamid, N. H. A., Nordin, S., Osman, R., Yusoff, N., & Gu, X. (2026).  
**Adaptive Local Outlier Factor.**  
*Evolving Systems*, 17(2), 44.  
https://doi.org/10.1007/s12530-026-09808-y

### BibTeX

```bibtex
@article{AlynLOF2026,
  author  = {Basheer, Muhammad Yunus Iqbal and Ali, Azliza Mohd and Hamid, Nurzeatul Hamimah Abdul and Nordin, Sharifalillah and Osman, Rozianawaty and Yusoff, Nooraini and Gu, Xiaowei},
  title   = {Adaptive Local Outlier Factor},
  journal = {Evolving Systems},
  year    = {2026},
  volume  = {17},
  number  = {2},
  pages   = {44},
  doi     = {10.1007/s12530-026-09808-y},
  url     = {https://doi.org/10.1007/s12530-026-09808-y}
}


---

## Author

- Muhammad Yunus Iqbal Basheer
- Azliza Mohd Ali
- Nurzeatul Hamimah Abdul Hamid
- Sharifalillah Nordin
- Rozianawaty Osman
- Nooraini Yusoff
- Xiaowei Gu
 
Adaptive Liza Yunus Nurzea Local Outlier Factor (AlynLOF)
