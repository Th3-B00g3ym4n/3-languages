# 3-languages
This is the same program with the same functionality but in 3 different languages 


```C++
#include <iostream>

using namespace std;

int main() {
  int guess;
  cout << "enter Guess: ";
  cin >> guess;

  cout << "guess: "<< guess << endl;
  
  
  srand((unsigned) time(NULL));
  
  for(int i=1; i<=5; i++){

    int x = rand() % 10;
  
    cout << x << endl;

    if(x == guess){
      i=5;
      cout<<"found!"<<endl;
      continue;
    }

  }
}
```


```Lua
io.write("Enter Guess: ")

guess = io.read("*n")
x = nil
math.randomseed(os.time())

for var=1,5 do
 x = math.random(1, 10)
  
  print(x)

  if x == guess then
    print("found!")

  end    
end
```

```python

import random

guess = int(input("enter guess: "))

for i in range(5):
  
  x = random.randint(1, 10)

  print(x)

  if x == guess:
    print("found!")
```
