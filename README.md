# logic-task-pass
# task Q-1
# method to remove i'th character
test_str = "NARMINMAJID"
print ("The original string is : " + test_str)

new_str = ""
for i in range(len(test_str)):
	if i != 2:
		new_str = new_str + test_str[i]

print ("The string after removal of character : " + new_str)


#task Q-2
for Number in range (1, 101):
    count = 0
    for i in range(2, (Number//2 + 1)):
        if(Number % i == 0):
            count = count + 1
            break

    if (count == 0 and Number != 1):
        print(" %d" %Number, end = '  ')
        
   #task-Q3     
        import collections
str1 = 'i am very busy today and next week'
d = collections.defaultdict(int)
for c in str1:
    d[c] += 1

for c in sorted(d, key=d.get, reverse=True):
  if d[c] > 1:
      print('%s %d' % (c, d[c]))
        
           
           
