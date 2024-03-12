# OptaPlanner-Quickstarts-v2.0

Steps to run Open source Opta Planner, I use a M3 Max, You will have to tweak it based on your operating system. 

Required (Have these pre installed before you run the code): 
* Maven
* Gradle
* Quarkus
* Java 17 - (Quarkus 3.8.2 does not support the use of the Java 21 on the M3 Max, I was running Java 21 and had to downgrade to 17 for this to work) 

I used IntelliJ, you can execute this even on terminal. 

1) Clone the git repo locally
2) locate the OptaPlanner-quickstarts -> Use cases -> select the use case as required. (Keep the required directory open)
3) Run the script to build using maven and execute it in developer mode
4) "mvn clean install" -> "mvn quarkus:dev"
5) You can see the output at Port 8080 (Switch the port if youre already using it or kill it) : http://localhost:8080/

Changes made to make it successfully run on an M3 Max:

1) Down graded from java 21 to 17
2) Quarkus 3.8.2 does not support certain builds on an M3,added a dependency in the parent POM file to update the quarkus version and fetch the required variables to run this build from the J Boss repo (Check the parent POM file if you want to review the changes).
3) Easy to use Opta Planner Quick start with just 2 scripting commands.

Future work: Opta Planner can be used to create optimized schedules for various use cases. 

Documentation: https://www.optaplanner.org/docs/optaplanner/latest/planner-introduction/planner-introduction.html 
