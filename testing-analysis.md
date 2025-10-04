• To what extent was your testing approach aligned to the software requirements? Support your claims with specific evidence.

Testing directly mapped to each requirement: Task ID validation (testTaskIdTooLong line 15, testTaskIdNull line 20), name validation (testNameTooLong line 25, testNameNull line 30), description validation (testDescriptionTooLong line 35, testDescriptionNull line 40), and service operations (testAddTask, testDeleteTask, testUpdateName, testUpdateDescription in TaskServiceTest.java).

• Defend the overall quality of your JUnit tests for the contact service and task service. In other words, how do you know that your JUnit tests were effective on the basis of coverage percentage?

44 total tests with 0 failures achieved 100% method coverage across all classes. TaskTest.java has 16 tests covering all validation paths, TaskServiceTest.java has 10 tests covering all service methods, with similar comprehensive coverage for Contact classes.

• How did you ensure that your code was technically sound? Cite specific lines of code from your tests to illustrate.

Validation testing ensures technical soundness: null handling (TaskTest.java line 21), boundary testing (TaskTest.java line 84 for max length), duplicate prevention (TaskServiceTest.java line 20), and graceful error handling (TaskServiceTest.java line 52 for non-existent updates).

• How did you ensure that your code was efficient? Cite specific lines of code from your tests to illustrate.

HashMap usage provides O(1) operations tested through direct key-based access: addTask (TaskServiceTest.java line 11), deleteTask (line 29), and updateName (line 45) demonstrate efficient lookup and modification without unnecessary object creation.
