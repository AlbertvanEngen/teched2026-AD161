# Exercise 4 - Push your agentic solutions to git and promote to production

In this exercise, we will push your solution to git and learn how to promote it to production

## Exercise 2.1 Push Solution to Git

After completing these steps you will have learnt how to connect your solution to git and push changes to git

1. 
2.	Insert this line of code.
```abap
response->set_text( |Hello ABAP World! | ). 
```



## Exercise 2.2 Promote Solution to Production

After completing these steps you will have learnt how to promote to production

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc = 0.
    response->set_status( i_code = 200
                     i_reason = 'Everything is fine').
    RETURN.
  ENDIF.

```

2.	Click here.
<br>![](/exercises/ex2/images/02_02_0010.png)

## Summary

You've now ...

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
