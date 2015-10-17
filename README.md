# php_check_syntax
Implementation of php_check_syntax through shell execution

When designing a PHP plugin system, a way is needed to check
a files syntax before including it. In my search I've found
that PHPs naive function for doing so, php_check_syntax()
was removed from PHP in version 5.0.5. It appears the only
way to perform a check is through the command line. This
is a wrapper function, simulating the interface of the 
original PHP function.

Even though I am not sure about the error messages 
provided by the original implementation, I am returning
what the shell execution returns as error message on
syntax error. 
