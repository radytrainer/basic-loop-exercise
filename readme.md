## Algorithm Basic Exercises

### Exercise #1
Enter string and display the result letter by letter.
```python
# Solution 1
text = input()
for i in range(len(text)):
    print(text[i])

# Solution 2
text = input()
i = 0
while i < len(text):
    print(text[i])
    i += 1
```

### Exercise #2
Enter string and find the letter "A" in text. if text contains a letter "A" display "Yes" otherwise display "No".
```python
# Solution 1
text = input()
isA = False
for i in range(len(text)):
    if text[i] == 'A' or text[i] == 'a':
        isA = True
if isA:
    print("Yes")
else:
    print("No")

# Solution 2
text = input()
i = 0
isA = False
while i < len(text) and not isA:
    if text[i] == 'A' or text[i] == 'a':
        isA = True
    i += 1
if isA:
    print("Yes")
else:
    print("No")
```