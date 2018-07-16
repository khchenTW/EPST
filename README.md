# Python source code and misc.

# Proposed and compared approaches:
- EPST.py contains the proposed approaches.
- bounds.py contains different bounds related to the Chernoff bound.
- task-generator.py contains the task generating routines, especially for generating MATLAB input [1].
- sort_task_set.py contains the task generating routines.
- mp-frVsProb.py is used to generate the results on multiprocessors.
- mp-frVsProb_dml.py is used to generate the results for l-consecutive misses on multiprocessors.
- cprta.py contains the approaches implemented in Python [1].
- scriptSimulations.m is the modified simulation executable from [1].
- dmp.m is almost the original one but the redundant output behavior is disable for readability.
- givenTaskSetFunction.m contains the function for using our generated input. The given input from taskset-matlabs100u60.m / taskset-matlabs100u70.m  should be renamed as "INPUT.m" in teh same folder.

# Experimental setup in the paper:
- timing.py contains the time measument routines.
- taskset-matlabs100u60.m / taskset-p10s100u60.txt are the input of shown results for utilization 60 generated by Uunifast.
- taskset-matlabs100u70.m / taskset-p10s100u70.txt are the input of shown results for utilization 70 generated by Uunifast.

# Heuristic example:
- simple_test.py heuristically demonstrates the usage of the proposed approaches.
- simple_approxError.py heuristically demonstrates the approx. error we made with given inputs.

# Error in my paper [2]
- in simple_test.py, P^A_1 and P^A_2 in the paper was reported as 10^-5. However in fact the results was all based on 10^-6. 
- Which real value s should be used in 

# Reference
- [1] D. Maxim and L. Cucu-Grosjean. Response time analysis for fixed-priority tasks with multiple probabilistic parameters. RTSS'13. The source code of CPRTA and the resampling feature is from here: https://who.rocq.inria.fr/Dorin.Maxim/tool.html
- [2] K. H. Chen and J. J. Chen, "Probabilistic schedulability tests for uniprocessor fixed-priority scheduling under soft errors," 2017 12th IEEE International Symposium on Industrial Embedded Systems (SIES), Toulouse, France, 2017, pp. 1-8.

