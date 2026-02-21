# telemetry_sbrc_2026

Dataset used in An Experimental Framework for Studying Non-IID Data in Federated Learning for Network Telemetry - SBRC 2026.

The datasets available in this repository are under the license CC-BY-4.0. The full terms are describe in the LICENSE.txt file in the root folder and also in the following link: https://creativecommons.org/licenses/by/4.0/

If you make any use of such datasets, please refer to it as follows:

The authors can be contact through: johny.ribeiro@ufu.br konstantinos.vandikas@ericsson.com maria.marquezini@ericsson.com chesteve@unicamp.br rafael.pasquini@ufu.br

# Description of dataset

Collected statistics for prometheus are stored in csv files. A csv file contains m rows of n features. Each row represents one observation and has a timestamp t indicating when the statistics were measured. Collected client metrics for Apache Cassandra are stored in {t100, t300, t500}_read.csv and {t100, t300, t500}_write.csv files together with the observation time t. During experiments, X and Y statistics are collected every second on the testbed.

The first row of all csv files brings the labels for the n features in X and the client metrics Y.
