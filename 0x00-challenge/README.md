# Fix-my-code-0

0-fizzbuzz.py
```python
if (i % 3) == 0:
	tmp_result.append("Fizz");
elif (i % 3) == 0 and (i % 5) == 0:
	tmp_result.append("FizzBuzz");
```
is rearranged to:
```python
if (i % 3) == 0 and (i % 5) == 0:
	tmp_result.append("FizzBuzz");
elif (i % 3) == 0:
	tmp_result.append("Fizz");
```

1-print_square.js
```js
size = parseInt(process.argv[2], 16)
```
conversion base is changed to default 10:
```js
size = parseInt(process.argv[2])
```

2-sort.rb
```ruby
result.insert(i - 1, i_arg)
```
index is corrected to be:
```ruby
result.insert(i, i_arg)
```

3-user.py
```python
def password(self, pwd):
	...
	self._password
def is_valid_password(self, pwd):
	...
	return ___.upper()
```
password (protected -> private) & (upper -> lower)

4-delete_dnodeint/
```c
(*head)->prev->prev = (*head)->prev;
free(*head);
...
```
is modified to be:
```c
(*head)->prev->next = (*head)->next;
...
free(*head);
```
