# Stacked Borrows

undone chapter.  
It would be preferrable if you read the paper on stacked borrows

Stacked Borrows is one of the methods used by Miri to detect undefined behaviour brought about by pointers (both references and raw-pointers).  
It is not a static method, it inspects a program dynamically.  

The problem with testing something based on dynamic info is that the program may not exhaust all paths. Such tests are not exhaustive.  
For this reason, you have to test a program dynamically while subjecting it to many test cases/data, hoping to stimulate all paths that the program-execution could have taken.  

The stacked Borrows mechanism is implemented dynamically because Unsafe pointers get affected by the runtime environment in a way that static analysis cannot cover.  

As earlier discussed, there are dozens of optimization dtrategies in the compiler world 
