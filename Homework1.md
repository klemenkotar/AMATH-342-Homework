# Homework 1
### Klemen Kotar / AMATH 342 with Eric Shea Brown

#### Part A - MATLAB Tutorial Problems

##### Exercise 4.1

INTEGRATOR STAGE 2: Write a code **integrator_2.m** which:

- defines a signal **signal_vector** (a vector of signal values at different timepoints) 
- defines a threshold **thresh**

and computes as its answer the first time that the cumulative sum of the signal crosses the threshold.

```
clear all

t=[1:10];
signal_vector = sin(t);
thresh = 0.5;

for n = t;
    if (signal_vector(n) > thresh);
        disp("We are crossing the threshold at time t = : " + signal_vector(n))
        break
    end;
end;
```


