# Telemetry SBRC 2026

This repository contains datasets created to use in our paper.

Collected statistics for prometheus are stored in csv files. A csv file contains m rows of n features. Each row represents one observation and has a timestamp t indicating when the statistics were measured. Collected client metrics for Apache Cassandra are stored in {t100, t300, t500}_read.csv and {t100, t300, t500}_write.csv files together with the observation time t. During experiments, X and Y statistics are collected every second on the testbed.

The first row of all csv files brings the labels for the n features in X and the client metrics Y.

If you make any use of such datasets, please refer to it as follows:

Johny Ribeiro and Konstantinos Vandikas and Maria Marquezini and Christian Rothenberg and Rafael Pasquini. "An Experimental Framework for Studying Non-IID Data in Federated Learning for Network Telemetry". In: Simpósio Brasileiro de Redes de Computadores e Sistemas Distribuídos (SBRC), 44. 2026, Praia do Forte/BA.

The authors can be contact through: johny.ribeiro@ufu.br konstantinos.vandikas@ericsson.com maria.marquezini@ericsson.com chesteve@unicamp.br rafael.pasquini@ufu.br


**Paper:** "An Experimental Framework for Studying Non-IID Data in Federated Learning for Network Telemetry"
**Abstract:**
_The increasing complexity of emerging 5G and 6G network environ-
ments has intensified the need for data-driven automation under heterogeneous
and dynamic conditions. Federated Learning (FL) is a promising paradigm in
this context. This paper presents an experimental framework to generate real-
istic Non-Independent and Identically Distributed (Non-IID) datasets through
controlled execution of a distributed service and telemetry collection, aiming to
improve the applicability of FL in network automation. Using Apache Cassan-
dra as a representative cloud-native application, we construct datasets exhibit-
ing temporal and structural heterogeneity. We statistically characterize these
datasets and evaluate their impact on regression models and horizontal fed-
erated learning using a Wide & Deep architecture. Results show that while
horizontal federation improves generalization compared to direct cross-dataset
transfer, its performance degrades under pronounced structural Non-IID condi-
tions, highlighting both its potential and limitations._

Two other repositories make up the entire environment for the experiments.

[Smartness Cassandra Stress RS](https://github.com/EricssonResearch/smartness-cassandra-stress-rs), contains code to our client and python scripts for our load generator and other utilities.

[Smartness Experiments](https://github.com/EricssonResearch/smartness-experiments), contains notebooks to analyse dataset and code to run the deep model used in our experiment and federated architecture.

# Badges considered

The authors consider the following badges as part of the evaluation process:

- Artifacts Available (SeloD)

# LICENSE

This software is under MIT-License. For more information please read LICENSE file.