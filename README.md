# Adversarial neural networks for Higgs physics
Applying Adversarial Neural Networks (ANNs) within the ATLAS experiment to improve the classification of Higgs boson events in the diphoton decay channel. In this work, the problem of mass sculpting is addressed when training a supervised classifier between Higgs signal and non-resonant background events.

<!--Mass sculpting can be addressed in multiple ways: -->

<!-- Re-weighting the background or signal input data to be uniform in the invariant mass -->

Overview presentation slides of this study can be found in <b>MPhys ANN overview.pdf</b>.

First need the <b>PowhegPy8EG_NNPDF30_VBFH125mc16a.csv</b> (Higgs->diphoton signal) and <b>Sherpa2_yyjj_njetGeq2_mjj_gt350.csv</b> (non-resonant background) datasets.

Sequence to run the notebooks to generate the results:
1. Generate ANN engineered features
2. Combine ANN features
3. ANN benchmark performance with 5% myy corr.
4. ANN training (hyperparameter optimisation)

layers.py and ops.py are local import files used in notebooks 3 and 4.
