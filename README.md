# ParMS Experiments

This repository contains the source code and experimental results for the **Partial Model Sharing (ParMS)**. The primary focus of this experiment is to explore the impact of sharing only a small portion of model parameters in the context of Deep Leakage from Gradients (DLG) attacks and to analyze the efficiency of such methods. Additionally, the repository includes an implementation of homomorphic encryption applied to a subset of the shared model parameters.

## Table of Contents

- [Overview](#overview)
- [Directory Structure](#directory-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Experiments](#experiments)
  - [DLG Experiments](#dlg-experiments)
  - [Efficiency Analysis](#efficiency-analysis)
  - [Homomorphic Encryption](#homomorphic-encryption)

## Overview

In this project, we investigate the effects of partial model parameter sharing on the vulnerability of deep learning models to DLG attacks. The repository also examines the efficiency of these methods and provides an additional layer of security through homomorphic encryption on the shared model parameters.

## Directory Structure

The repository is organized as follows:

```
ParMS/
├── DLG_attacks/
├── Efficiency/
│   └── HE/
├── README.md
```

- **DLG_attacks/**: Experiments related to DLG attacks with full and partial model access.
- **Efficiency/**: Analysis of the model's efficiency when sharing a small portion of model parameters.
  - **encryption/**: Implementation of homomorphic encryption on the shared model parameters.

- **README.md**: This file, providing an overview and usage instructions for the repository.

## Installation

To set up the environment, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/ParMS.git
   cd ParMS
   # go into any of the experiments and run the jupyter notebook
   ```

## Usage

You can run the experiments and analyze the results by executing the scripts provided in the above directory. Each experiment is configured as a Jupyter notebook, which you can run directly.
## Experiments

### DLG Experiments

The DLG experiments explore the impact of sharing different portions of the model on the success of DLG attacks. The experiments are divided into two main categories:

- **Full Model Access**: Where the attacker has access to the entire model.
- **Partial Model Access**: Only a portion of the model parameters are shared at each round.

### Efficiency Analysis

In this set of experiments, we analyze the efficiency of training and communication when only a subset of model parameters is shared. The aim is to understand the trade-offs between security and performance.

### Homomorphic Encryption

We implemented homomorphic encryption to secure the subset of model parameters shared during training. This section of the repository includes the code for encryption and the experiments analyzing its impact on security and efficiency.
