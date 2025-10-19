[Syllabus](https://faculty.cc.gatech.edu/~ladha/S24/3510/)
Exams are take home and open note. **This means they may be harder**

money

HW released thursday due monday.


```
We can a counter to keep track of the total number of number outside the range we have found.
Split the array into two halves $$A_L$$ and $$A_G$$. With all the half with larger numbers being in $$A_G$$. 

If the smallest number in $$A_G$$ is greater than $$u$$ we add the size of $$A_G$$ to the counter. Otherwise, we recursively call this function on $$A_G$$ with the same range $$[l,u]$$ then add what we get to the counter.
If the largest number in $$A_L$$ is less than $$l$$ we add the size of $$A_L$$ to the counter. Otherwise, we recursively call this function on $$A_L$$ with the same range $$[l,u]$$ then add what we get to the counter.
Our counter has the answer.

THIS IS WRONG FIX IT LATER
```