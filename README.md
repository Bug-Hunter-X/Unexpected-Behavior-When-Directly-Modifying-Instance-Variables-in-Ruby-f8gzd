# Ruby Instance Variable Modification Bug

This repository demonstrates a potential issue in Ruby when directly modifying instance variables using `instance_variable_set`. While it might seem convenient, this approach can lead to several problems:

* **Bypass of Getter/Setter Methods:** It sidesteps any validation or logic within getter and setter methods, potentially leading to inconsistent state or unexpected results.
* **Reduced Maintainability:** Direct manipulation makes code harder to understand and maintain, as it's difficult to track all modifications to instance variables. 
* **Debugging Challenges:** Debugging becomes more difficult because the standard flow of accessors is disrupted. 

The provided code showcases the issue and suggests a better approach using accessor methods.