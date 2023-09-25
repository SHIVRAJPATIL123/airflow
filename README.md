# airflow
 Help to manage multiple Data pipelines
benefits 1 everything in python and dynamic ,2.scalblity 3. user interface 4.Extensibilty -you can add multiple plugins you needed 
components 
1.web server - flux python web server that allows you to the use interface  
2.scheduler  - shedule your tasks and your data pipeline 
3.Metastore  - Data base compatable with the sequal like postgres,mysql,oracle-db contain metadata related to the pipelines and the task 
4.Triggere - Allows you to run specific kind of Task .
5.Executor - Defines How and on which pod your task is execuated 
Queue - your task push in it to executed in an order.
Worker - where your task are effectively executed .
****
DAG -- Directe asicallty Graph
Operator - It is nothing but like the task 
1. Action operator-to run the script inside the db 
2. Transfer operator-transfer the data to db 
3. Sensor operator -run certain task after certain task completed
4. command  
4.airflow db init
6.airflow db upgrade
airflow db reset
airflow dag list
airfolw tasks list dag-id
airflow dag trigger -e 2020-01-01 dag-id ........schedule the tasks
aieflow create user -u adimin -p admin -co........remaning file url
Airflow UI description------------------------------------------------------------
left trigger -- used to pause or unpause the Dag
neme of the pipeline and the tags in ehe case of multiple pipelines
owner - airflow or name of teams
 Runs - sucess, running or fails, ststus of past and current dag runs 
schedule -  daily *****
Last Run - execuation date last
Recent Task -success,running,fail,ststus of the task for thr last dag run
Actions - Trigger manually , Refresh,delete-only delete metadata in the metastore not delete the file
Links - to get access to other views of the data pipelines like Trees,Graph etc
by clicking on the dag by default we goes to the tree view -gives the history of the dag runs 
cirle - gives information about the dag runs
square gives the information about the corresponding tasks
 Graph  view - gives the current or latest dag runs
Gantt View - useful if the Task taking large times or the task can be executed parallel or not
Modular View -By clicking the Task inside the Graph view you get the detail information about the Task showed in the modular view like logs
clear- clear you r task to rerun or retry the tasks
Mark Failed or Mark Success - 
