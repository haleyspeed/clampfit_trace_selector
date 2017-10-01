# clampfit_trace_selector
Function to automatically generate a list of traces for analysis in Clampfit (part of the Molecular Devices PClamp suite for electrophysiology data acquisition and analysis). Default is set up for averaging or basic statistics of raw paired pulse ratio traces presented in non-sequential order. 

### The three variables that may need to be changed are:
- *start* -> this is the first sweep you want to analyze
- *intervals* -> this is the number of interstimulus intervals you measured
- *reps* <- this is the number of traces you want to analyze per interstimulus interval

### The default for the Powell Lab Paired Pulse Cycles protocol (Speed et al., 2012, 2013, 2015) are:
- *start* <- 1
- *intervals* <- 6 (in pseudorandom order: 50 ms, 500 ms, 100 ms, 80 ms, 30 ms, 200 ms)
- *reps* <- 10 

### Sample output with default values
~~~~
[1] "t1,t7,t13,t19,t25,t31,t37,t43,t49,t55"
[1] "t2,t8,t14,t20,t26,t32,t38,t44,t50,t56"
[1] "t3,t9,t15,t21,t27,t33,t39,t45,t51,t57"
[1] "t4,t10,t16,t22,t28,t34,t40,t46,t52,t58"
[1] "t5,t11,t17,t23,t29,t35,t41,t47,t53,t59"
[1] "t6,t12,t18,t24,t30,t36,t42,t48,t54,t60"
~~~~
