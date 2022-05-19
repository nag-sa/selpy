# Selnium with Python
- **To install pytest** --> go to  cmd --> pip install pytest
- To check version of pytest installed --> pytest --version
- Naming convesion for pytest file --> will strats from ---> test_demo.py or _testdemo.py   (_test or test_ is mendatory)
- pytest programs/code should be written in form of function and warreped in method. (myname is a method here)
    ```
    EX.  def myname():
        print("my name is saurabh")
    ```    
- If the method name is same (like one more def myname(): in a same test_demo.py file), then it gets overwritten. Instead for two we will get result for one method not for two. 
- Better to run/execute all programs/scripts from terminal(command prompt)
- To execute from cmd ---> go to cmd ---> path of folder where prog/scripts are placed (folder location)---> py.test (This command will run all the scripts available in your folder and file starts from test_ or _test)
- To execute from cmd ---> go to cmd ---> path of folder where prog/scripts are placed (folder location)---> py.test -v (-v stands for verbose,or more info, it gives result in some descriptive way)
- To execute from cmd ---> go to cmd ---> path of folder where prog/scripts are placed (folder location)---> py.test -v -s (-s stands for print the logs, and gives console o/p, gives no. of test cases pass, fail)
- To execute any specific file/testscript/ from cmd --->path of folder where prog/scripts are placed (folder location)---> py.test test_demo1 -v -s  (test_deno is a file we want to sepcifically execute)
- Important --> your test case name is nothing but your method name avaiable in your test file, So while wriring testcases give some meaning full name to your method, as they will represent your testcase name.
- We can group our testcases based on method name, and to run specific testcases based on method name/testcase name, run below command from cmd:
   1. Go to cmd ---> path of folder where prog/scripts are placed (folder location)---> py.test -k creditcard -v -s  (-k stands for method name execution)(where creditcard is method name, so all testcases named with creditcard will run)
- we can mark (tag) tests and then run with command -m  ---> cmd --->folder location--->py.test -m smoke -v -s (-m stands for mark and smoke is a tag associated)
for above(pt.16) execution we need to import pytest and give name like `@pytest.mark.smoke`

