Tasks to answer in your own README.md that you submit on Canvas:

1.  See logger.log, why is it different from the log to console?.

The logger.log file includes a FINER parameter that does not appear in the console. In the logger properties file, only INFO 

1.  Where does this line come from? FINER org.junit.jupiter.engine.execution.ConditionEvaluator logResult Evaluation of condition [org.junit.jupiter.engine.extension.DisabledCondition] resulted in: ConditionEvaluationResult [enabled = true, reason = '@Disabled is not present']

This line is the 4th line in the logger.log file. It appers

1.  What does Assertions.assertThrows do?

assertThrows takes a lambda expression and checks if an expression will be thrown. If no exception is thrown, then the method will fail. 

1.  See TimerException and there are 3 questions
    1.  What is serialVersionUID and why do we need it? (please read on Internet)

    This is an identifier that is used for serialization/deserialization of an object of a Serializable class. 

    2.  Why do we need to override constructors?

    We call the super method in these constructors so that we can display detailed messages with our exceptions. 


    3.  Why we did not override other Exception methods?	

    Exception extends from the Throwable class and we don't need to override those methods. 

1.  The Timer.java has a static block static {}, what does it do? (determine when called by debugger)

A static block is used for initializaing static variables within a class. 

1.  What is README.md file format how is it related to bitbucket? (https://confluence.atlassian.com/bitbucketserver/markdown-syntax-guide-776639995.html)

.md is a file format that contains plain-text that can be customized in terms of font-size & display options

1.  Why is the test failing? what do we need to change in Timer? (fix that all tests pass and describe the issue)

The Test is failing because the statement in assert throws is not throwing an exception. This is because the expected exception is not being thrown becuase it is in the try/catch/finally block. we can fix this by just moving the if statement outside of the try/catch/finally block. 

1.  What is the actual issue here, what is the sequence of Exceptions and handlers (debug)

The Try/Catch/Finally was expecting an Interruptede Exception rather than a TimerException which is why the assertThrows was failing because it never catches the TimerException. 

1.  Make a printScreen of your eclipse JUnit5 plugin run (JUnit window at the bottom panel) 

done

1.  Make a printScreen of your eclipse Maven test run, with console

done

1.  What category of Exceptions is TimerException and what is NullPointerException
1.  Push the updated/fixed source code to your own repository.