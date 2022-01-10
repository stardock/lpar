# lpar
AIX Lpar performance reviw


Q: How many vCPUs my LPAR will can use?  
```
the general rule for AIX is as follows:

Mode = (Capped | Uncapped)

If Capped then you read the
 
Entitled Capacity = xxxx

If Uncapped then you read the
 
Online Virtual CPUs = xxxx

So in your case, its Uncapped, so we read the Online Virtual CPUs : 1

So 1 vcpu is the answer.
```  

Check the Lpar setup configure:
`lpar -i`


Ref: https://www.ibm.com/mysupport/s/question/0D50z00005pf42uCAA/how-many-vcpus-my-lpar-will-can-use?language=en_US  
