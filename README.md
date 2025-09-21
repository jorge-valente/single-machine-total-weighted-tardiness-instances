# Instances for the Single Machine Total Weighted Tardiness Scheduling Problem
This repository contains training and test instances for the single machine total weighted tardiness scheduling problem.

More specifically, the instances are those proposed and described in the following paper:

Ana Sofia M. Martins, Jorge M. S. Valente and Jeffrey E. Schaller (undergoing the second revision in International Transactions in Operational Research), "A Computational Evaluation of New and Existing Dispatching Rules for the Single Machine Total Weighted Tardiness Problem".
&nbsp;

&nbsp;

The zip files "training_set.zip" and "test_set.zip" contain the training  and test instances, respectively.

All instances are in CSV format, and named according to the following convention: *n*-*T*-*R*-*i*, where *n* is the number of jobs, *T* is the value of the tardiness factor, *R* is the value of the due date range factor, and *i* is the number of the instance (for a given combination of *n*, *T* and *R*). So, and as an example, instance 250-0.2-0.4-5  is the fifth instance among those with 250 jobs, a tardiness factor of 0.2 and a due date range factor of 0.4.

For each combination of *n*, *T* and *R*, there are 10 instances in the training set and 100 instances in the test set. So, for any given combination of *n*, *T* and *R*, *i* goes from 1 to 10 in the training set and from 1 to 100 in the test set.

The following values were used for *n*, *T* and *R*:

*n*: 50, 100, 250, 500, 1000, 2000

*T*: 0.2, 0.4, 0.6, 0.8, 1.0

*R*: 0.2, 0.4, 0.6, 0.8, 1.0
&nbsp;

&nbsp;

The first line of each file is the following header: job_index,processing_time,tardiness_unit_time_cost,due_date

The data for each job is in the next lines, one job per line, and in the order indicated in the header (index, processing time *pj*, tardiness unit time cost *wj* and due date *dj*).

The integer times *pj* were generated from a uniform distribution U(1, 100).

The integer tardiness unit time costs *wj* were generated from a uniform distribution U(1, 10).

The integer due dates *dj* were generated from a uniform distribution (*P* X (*1* - *T* - *R*/2), P X (1 - *T* + *R*/2)), where *P* is the sum of the processing times *pj* of all jobs.
&nbsp;

&nbsp;

As noted below, a CC-BY-SA-4.0 license has been applied to these instances. We please ask you to comply with the terms of this license, and to always perform a proper attribution if you use these instances.
For any questions, please contact the corresponding author, Jorge M. S. Valente (jvalente *at* fep.up.pt).
&nbsp;

&nbsp;

# License
[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
