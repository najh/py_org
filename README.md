# py_org

py_org is a Python 3 script to generate [Org](https://en.wikipedia.org/wiki/Org-mode) files from JSON inputs.

## Usage:

```python
import py_org

def parse_json(filename):
    f = open(filename, "r")
    contents = f.read()
    q.add_parse(contents)
    f.close()

def write_output(path, contents):
    f = open(path, "w")
    f.write(contents)
    f.close()

q = py_org.Org()
parse_json("input1.json")
parse_json("input2.json")
write_output("journal.org", str(q))
```