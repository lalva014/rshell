# rshell
Assignment 4

The purpose of this assignment is contruct a shell in c++

The Bugs: 
  If too many semicolons are input into the shell, the program putputs an out of range error/crash. the reason is the way we take out input from the command. we couldn't found away to make this work. the exit only works after using it multiple times. if you run the program then exit right away. it will exit but you processed by a command such as ls. the termanl will not exit. you have to enter it multiple times in order for it to work. another thing when we try typing echo &. the terminal did not output the & to the termanl. it outputs and out of range vector. the same thing happen with the || but it doesnt iwth the &&. we also notice that it work for the semi. so if we echo ;  it echos just a space. we also found by inputing into the terminal " ls ls", we got an error. Another thing that strtoke. every time we used it, we couldn't figure it out how to delete the allocated memory. if we put as many && with commands and then echo  hello; the terminal would not complie the last hello; 

Update:
  The are some errors when calling the test command. there is an error when outputing the error for a test command for example if when test command outputs "command not found" is out put "test not a file or directory " instead. semi colons cannot be spaced like for example ls;ls will only execute one ls but the other.this applies to every case that semi colomn doesnt have a space. if the semi colomn is at the end of the second command it would also not excute for exampla ls ;ls. this is true for every case that has the semicolomn in this position. there is an error in a nested parentheses, if there are two parentheses they must be next two each other and not seperated by space. There still some memory leaks that need to be address because we allocate new memory but failed to to deallocate memory. There probably more bugs in the program that we have not caught but they do not seems to impact the overall performance.

Update 2(current):
