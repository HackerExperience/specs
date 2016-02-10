# Processes

Processes, also known as tasks, are actions performed by you that need to be calculated/processed somehow, and therefore some time will take until the process is completed. It can take from as little as 4 seconds to days or weeks, depending of the action you are performing and others factors.

According to the action being performed, each process follows one of the three scheduling algorithms described below. The way resources are allocated also differs from process to process.

### Scheduling Algorithms

#### Transient

The process has a clear goal and will reach an end after sometime, causing a side-effect.

Example: Deleting a file.

#### Persistent

The process runs forever and won't cause any side-effects. It's usually a secondary factor of other actions. 

Example: Firewall passively protecting from connections.

#### Iterative

The process runs forever, causing side-effects from time to time. The time required to cause each side-effect usually increases exponentially. 

Example: Recovering a specific log (which might have received several prior editions)


### Resource Allocation

#### Static

The process will always use the same amount of resources. Those resources are reserved by the process.

#### Dynamic

A process might allocate unused resources dynamically, according to the total of  resources available and process priority.

#### Variadic

A variadic process combines both static and dynamic allocations by reserving a fixed amount of resources (static) and allowing the player to increase the amount of resources being used (dynamic), thus decreasing the total time required to complete the task.

### Work Units

Every process need some time to cause a side-effect. The required time is calculated through work units. Usually, all processes of same type, under the same conditions and environment, will require the same amount of work units. The difference lies on the user hardware, which can compute more or less work units per second. This is analogous to hardware clock rate.

### Resource Management

#### Process Priority

A process can have any of the following priorities: Lowest, Low, Normal, High, Highest. Changing the priority of a process is not possible for statically-allocated processes.

#### Pausing/Resuming

The player can pause and resume any process, at any time, without losing the computed work units. Pausing a process will free any reserved resources.

