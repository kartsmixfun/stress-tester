## This file gives you a description of every file present inside the testing folder 

### brute_test.cpp

This file contains an incorrect (the code that you want to test against someone's code) or brute force-based code. Please note this thing carefully file format should be exactly like this as shown below:

```
#include "h1.h"
_s

_1 // You can use _1 if you have no test cases I mean you have to run your code just for one sample case otherwise _2 means you have one or more test cases to be tested which is defined at the first line of ip.txt file.
```

While writing your code doesn't include ```main``` or any header files as this all has been done inside ```h1.h``` header file, also note it carefully that on expanding 
this code will look like this:

```
#include "h1.h"
void solve()
{

}
int main()
{
solve();
// some code snippet (leave it it is just used for)
}
```

So when you are writing any piece of code between ```_s``` and ```_1``` basically you are writing it inside the ```solve()``` function as per definitions of ```#define```

One may go through the ```h1.h``` header file to observe each and every #defines and structuring if interested, however, you are free to put your code the way you want.

### optimal_test.cpp

This file contains a correct (someone's code that you want to test against your own code) or optimal approach code of some problem written by you.

Rest is similar to brute_test.cpp

### test_case_generator.cpp

Used to generate test cases, please note as test cases format varies too much hence it is not generalized for every problem one has to write it on his own.

The above file describes a test case format in which we have the first line as a total number of test cases and every tc have the first line as the number of elements in an array then the second line contains array elements.

### brute_test_out.txt and optimal_test_out.txt 

Files containing the o/p generated by respective ```.cpp``` files

### chromedriver.exe

Used for selenium browser automation 

### h1.h 

The header file is written by me as per my c++ template however it is mandatory to keep it where it is included in ```.cpp```

### in.txt 

i/p file note here you can manually copy the tcs from somewhere or write on your own or generate it via ```test_case_generator.cpp``` file.