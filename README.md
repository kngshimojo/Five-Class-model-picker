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

Files
----------------------------------------------
- ./model/model_epoch_143.pt
  - Pretrained FC model
- ./tutorial_fc_model.ipynb
  - Sample program to use the pretrained weights in the model directory, where were obtained through training with the JMA Unified dataset for 2014-2022.

References
----------------------------------------------
- Zhu and Beroza (2019), doi: 10.1093/gji/ggy423
- The paper detailing these released models is currently under peer review for an academic journal.
