 **每日学习日志模板**
```markdown
# 2026-02-03 - PyTest Fixtures

## 1. Learned
- Difference between function and class fixtures
- Scope: function, class, module, session
- Autouse fixtures run automatically without being requested

## 2. Example / Code Snippet
```python
import pytest

@pytest.fixture
def sample_data():
 return [1, 2, 3]

def test_sum(sample_data):
 assert sum(sample_data) == 6
