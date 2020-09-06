### Scripts used to run the project ###

**code_only_run**

Runs only MPCC and Boundary Estimation code sections.

If visualisation pre-processor statement active, code will hang as no rosviz process available to receive visualisation messages.

**rosviz_start**

Runs MPCC and Boundary Estimation code sections AND rosviz visualisation code.

Significant performance hit, so only use if visualisation desired.

**rqt_start**

Runs MPCC and Boundary Estimation code in rqt.

For this, rqt needs to be installed (http://wiki.ros.org/rqt), in which the plot and rviz panels are open. In plot, the solve_times and mpcc_times subscribers need to be specified.

**"r_" prefix**

Compiles MPCC and Boundary Estimation code sections in release mode rather than default.

**"v_" prefix**

Compiles MPCC and Boundary Estimation code sections in debug mode rather than default and runs via Valgrind.

### rviz config file ###

**rviz_config_MPCC_BE** needs to be set as the default rviz config file in order to be able to run the simulation. This contains all the needed subscribers.
