## Five-class classification model by PhaseNet-based model
----------------------------------------------

Overview
----------------------------------------------
The five-class (FC) model is a PhaseNet-based neural network developed for integrated detection and classification of ordinary earthquakes and low-frequency earthquakes (LFEs).

Unlike the original PhaseNet(Zhu and Beroza, 2019), the FC model predicts probabilities for five classes:

| Class | Description |
| :-------------- | :-------------: |
| OP | P phase of ordinary earthquakes |
| OS | S phase of ordinary earthquakes |
| LP | P phase of LFEs |
| LS | S phase of LFEs |
| Noise | Background Noise |

For model training, we used event waveform data corresponding to picking values in the JMA unified hypocenter catalog (hereafter, JMA catalog), which were compiled by Naoi et al. (2024).

Files
----------------------------------------------
- ./model/model_epoch_143.pt
  - Pretrained FC model obtained by training with the JMA Unified dataset for 2014-2022.
- ./tutorial_fc_model.ipynb
  - Sample program to use the pretrained weights in the model directory.
References
----------------------------------------------
- Zhu and Beroza (2019), doi: 10.1093/gji/ggy423
- Naoi et al. (2024), doi: 10.1186/s40623-024-02091-8
- The paper detailing these released models is currently under peer review for an academic journal.
