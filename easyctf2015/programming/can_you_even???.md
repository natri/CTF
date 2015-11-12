#problem
Use the programming interface to complete this task. You'll be given a list of numbers.
Input: A list of numbers, separated by commas.
Output: The number of even numbers.
Read the input from a file called can-you-even.in that's in the current working directory, and then write your output to a file called can-you-even.out.
````
f1 = open('can-you-even.in','r')
input = f1.readline().split(',')
total = 0
for x in input:
  if int(x) % 2 == 0:
    total = total + 1
f1.close()

f2 = open('can-you-even.out','w')

f2.write(str(total) + '\n')
f2.close()
````
