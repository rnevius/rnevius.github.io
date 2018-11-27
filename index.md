---
---

# This is a test.

```python
from django.db import models


class Car(models.Model):
    """This is some documentation."""
    name = models.CharField(max_length=255)


    def __str__(self):
        return self.name
```

