# RCplex


A Patched version of RCPLEX to acutally make installing possible + the ability to use multithreading. Tested on WSL with 

```
R CMD build Rcplex

R CMD INSTALL Rcplex_0.3-3.tar.gz --configure-args="--with-cplex-dir=/opt/ibm/ILOG/CPLEX_Studio201/cplex"

```

if using ROI plz run `ROI_plugin_register_solver_control("cplex", "threads", "X")` before any optimisation occurs for access to the `threads` param
