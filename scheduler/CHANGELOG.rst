^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package scheduler
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.0.1 (2014-10-24)
------------------
* Adding ncurses rosdep and also correct mongodb component order.
* Tidying up package and cmake files.
* Added absolute paths to libraries to ensure that dependent projects get correct linking.
* This simply bulk replaces all ros_datacentre strings to mongodb_store strings inside files and also in file names.
* Added argument for number of instances of scheduler to use.
* updated for better multi support
* Added first task logic to scheduler.
  Also made replay script work with mulitple parallel schedulers.
* Scheduler supports a task, which has the flag NOW
* Fixed issue when no file is given for saving in scheduler
* Added time meaurement for generating constraints and added generation of random schedules
* Adding timeout to scheduler.
* Added 1 minute timeout to scheduler.
* Replay script moves start of task set to 0 to make metrics more sensible.
* Integrated @mudrole1's scheduler changes into node.
* Added file to replay scheduling problems from datacentre
* Added parameter to prevent problem saving.
* Added parameters to scheduler_node and added options, when no parameter is set
* Versions of scheduling algorithm can be chosen now + logging of results to file
* Fixed minor scheduling issues.
  1) Made service calls thread safe.
  2) Fixed order of calls in cancellation
  3) Removed blocking assumption in demand task in scheduler
  4) Changed bounding of tasks based on current execution time.
* Fixed minor scheduling issues.
  1) Made service calls thread safe.
  2) Fixed order of calls in cancellation
  3) Removed blocking assumption in demand task in scheduler
  4) Changed bounding of tasks based on current execution time.
* Reduced calls to mdp time stuff.
* cacheing results, but seems to not be having much effect
* Added logging of scheduling problems to datacentre.
  Inefficient use of space, but faster for CPU (duplicating db content with tasks).
* Added logging of scheduling problems to datacentre.
  Inefficient use of space, but faster for CPU (duplicating db content with tasks).
* Quick fix for empty node ids waiting for `#41 <https://github.com/strands-project/strands_executive/issues/41>`_
* getting scheduler to call right expected time service
* first version of mdp policy execution
* Clarified behaviour around rescheduling after a demand.
  Dropping of out-of-bounds additional tasks are not handled separately to out-of-bounds previously scheduled tasks.
* reverting change in scheduler
* getting example task routines to have proper start and ending points
* Removed pre-variables, enlarged handling of preceding constraints
* Changes for on demand tasks.
  Added service for on-demand tasks.
  Restructued scheduled executor to separate new and old tasks, with the aim to allow this to be used to recover tasks overridden by on-demand requests.
* Adding prism and initial prism-ros interaction
* Delayed execution tasks now working correctly with timer.
* Publishing schedule and handling scheduler fail.
* Set up for just patrolling. Launch file printing to screen sensible amounts.
* Fixed bug, that time t was preceeding start of a task
* Compilation under linux now.
* Looking to add time delays to scheduler and executor, but bug found in scheduler.
* Setting up scheduler tests.
* Running scheduler, receiving back at execution framework.
* Working calls to the scheduler!
* Scheduler C++ node is now called with tasks.
* Adding infrastructure for scheduled execution.
* Compiled from scratch.
* A working compiler with lots of cmake hacks.
* Contributors: Bruno Lacerda, Lenka Mudrova, Nick Hawes
