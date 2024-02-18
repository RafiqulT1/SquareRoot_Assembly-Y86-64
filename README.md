# Square Root (Assembly Y86-64)
>+ ### About This Project 
>> This is a squire root calculator made with assembly Y86-64. Which will calculate the squire root of your desired number.       
In this project I collaborated with @valtteri98. We wanted to learn a low-level coding language to get a richer understanding of the underlying computer architecture.
>+ ### Run Squire Root code
>> To run this code, you can use Y86-64 simulator.   
Y86-64 Simulator: https://boginw.github.io/js-y86-64/
>+ ### Squire Root Algorithm 
```
Squire Root algorithm which I have converted into assembly.
CODE IN C 
// num is the number which square root is calculated
// res is the result
int32_t res = 0;
int32_t bit = 1 << 16; 

while (bit > num) {
   bit >>= 2;
   }
   
while (bit != 0) {
   if (num >= res + bit) {
      num -= res + bit;
      res = (res >> 1) + bit;
   } else {
      res >>= 1;
   }
   bit >>= 2;
}
```
