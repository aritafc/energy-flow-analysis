# New event-wide strategies for increasing di-Higgs efficiency with Machine Learning at trigger level
Ana Rita Carvalho (ana.rita.carvalho@tecnico.ulisboa.pt)

This work explores Energy Flow Polynomials (EFPs) computed at event-level and studies their sensitivity to different event topologies, discriminating four-jet HH->4b signal events from dijet background, for an environment with pile-up of 200 proton-proton collisions per bunch crossing. The performance of a supervised linear classifier trained with the EFPs is benchmarked by two alternative techniques: a standard multijet trigger with a transverse momentum cut and a Deep-Sets-based neural network, implemented with Particle Flow Networks (PFN) . 

The datasets for signal and background can be accessed [here](https://data.mendeley.com/datasets/v9z86dp9mv/1 . Each file contains two jets collections: the first, which we refer to as offline jets, calculated by the particle flow anti-kt algorithm; the second, corresponding to L1 trigger jets, is calculated with a simplified sliding window algorithm. The notebook `Offline_L1Trigger_Jets.ipynb` contains the analysis for these two jet collections.

A third set of jets was obtained by smearing the transverse momentum of offline jets to reproduce the expected resolution of the HLT, using information from the [ATLAS Public Jet Trigger Plots](https://twiki.cern.ch/twiki/bin/view/AtlasPublic/JetTriggerPublicResults#Transverse_momentum_of_High_Leve). The notebook `HLT_Trigger_Jets.ipynb` contains the analysis for HLT jets.

In order to run the notebooks, it is only necessary to download the datasets, and the file that contains the information used in the smearing, `plot-data.csv`. If the notebook is run locally, the packages mentioned in the notebooks preamble are also needed (namely the EnergyFlow package).
