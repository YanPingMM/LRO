You can simply define your cost in a seperate file and load its handle to fobj 

The initial parameters that you need are:
fobj = @YourCostFunction
dim = number of your variables
max_iter = maximum number of generations
searchagents = number of search agents
lb=[lb1,lb2,...,lbn] where lbn is the lower bound of variable n
ub=[ub1,ub2,...,ubn] where ubn is the upper bound of variable n
If all the variables have equal lower bound you can just define lb and ub as two single number numbers

To run LRO: [Best_Score,Best,convergence_curve]=LRO(searchagents,max_iter,lb,ub,dim,fobj)
