## Overview

This directory contains experiments related to Deep Leakage from Gradients (DLG) attacks, focusing on scenarios with full model access vs partial model parameter sharing. Specifically, we explore the effects of sharing only a small portion of model parameters during each training round.

### Experiment Design

To simulate partial model parameter sharing, we partition the model into three segments: lower, middle, and upper. During each training round, only one of these segments is shared.

### Experiments related to varying the lower segment

You can adjust the amount of the lower segment that is shared by modifying the `expose_ratio` parameter. The `expose_ratio` is defined as `1/N`, where `N` represents the total number of model partitions.
