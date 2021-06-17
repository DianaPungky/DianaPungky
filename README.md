<!-- Zero width character is used to put extra blank lines before and after code -->

<h3>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple = ("HTML", "PHP", "JavaScript", "Java", "C++", "VB.net", "Python")
    databases   : tuple = ("Mysql")
    framework     : tuple = ("Codeigniter", "Laravel")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```
</h3>
