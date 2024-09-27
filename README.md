# LSST API query

## A small python helper for querying Solar System data available from the Rubin Science platform.

1) Install the requirements
```
pip install -r requirements.txt
```

2) Add your API token in a .env file in the lsst_query folder. Make sure when creating the key you tick all your necessary permissions.

3) Example usage of the query helper function:
```python
from db import query

id_ = query(f'''select distinct sso.ssObjectId from dp03_catalogs_1yr.SSObject as sso LIMIT 1''')
```
