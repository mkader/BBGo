* A deadlock occurs when two or more transactions are waiting for each other to release locks on resources they need to continue processing. This results in a situation where neither transaction can proceed, and they end up waiting indefinitely.
* Coffman Conditions - describe four necessary conditions that must be present simultaneously for a deadlock to occur:
  1. Mutual Exclusion
  1. Hold and Wait
  1. No Preemption
  1. Circular Wait

* Deadlock Prevention
  1. Resource ordering: impose a total ordering of all resource types, and require that each process requests resources in a strictly increasing order.
  1. Timeouts: A process that holds resources for too long can be rolled back.
  1. Banker’s Algorithm: A deadlock avoidance algorithm that simulates the allocation of resources to processes and helps in deciding whether it is safe to grant a resource request based on the future availability of resources, thus avoiding unsafe states.

* Deadlock Recovery
  1. Selecting a victim: Most modern Database Management Systems (DBMS) and Operating Systems implement sophisticated algorithms for detecting deadlocks and selecting victims, often allowing customization of the victim selection criteria via configuration settings. The selection can be based on resource utilization, transaction priority, cost of rollback etc.
  1. Rollback: The database may roll back the entire transaction or just enough of it to break the deadlock. Rolled-back transactions can be restarted automatically by the database management system.
 
<img src="https://substack-post-media.s3.amazonaws.com/public/images/ddc67431-bad7-472c-85ac-70712ae88d02_1280x1664.gif">
