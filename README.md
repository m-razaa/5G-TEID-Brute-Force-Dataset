# 5G TEID Brute-Force Attack Dataset

This repository provides the machine-learning-ready dataset used in our paper accepted at **DIMVA 2026**: *Protocol-Aware Detection of TEID Brute-Force Attacks in 5G Networks*.

## 📖 Overview
Current public datasets often lack visibility into 5G user-plane tunneling semantics. To address this, we generated a novel dataset using a Docker-based OpenAirInterface (OAI) 5G testbed. Traffic was captured on the N3 interface (gNB ↔ UPF), providing direct visibility into GTP-U encapsulated flows.

The dataset includes benign background traffic (HTTP, Video, Control Signaling) and adversarial traffic generated via a two-stage TEID brute-forcing and payload injection attack. 



## 💾 The Dataset
The `5G_TEID_Attack_Dataset_Clean.csv` file contains roughly 8,000 flow records. It includes 72 features comprising both generic TCP/IP flow statistics and extracted GTP-aware tunnel semantics (e.g., TEID switch rates, payload percentiles, and directionality imbalance).



## 📝 Citation
If you use this dataset in your research, please cite our paper:
```bibtex
@inproceedings{raza2026protocol,
  title={Protocol-Aware Detection of TEID Brute-Force Attacks in 5G Networks},
  author={Raza, Muhammad and Rif{\`a}-Pous, Helena and Garrigues Olivella, Carles},
  booktitle={Proceedings of the Conference on Detection of Intrusions and Malware \& Vulnerability Assessment (DIMVA)},
  year={2026}
}
