# Use env variables

Create a .env file in parent folder

``` text
# environment variables defined inside a .env file
GCP_PROJECT_ID=my-project-id
SERVICE_ACCOUNT_FILE=path/to/serviceAccountCredentials
STORAGE_BUCKET_NAME=my-super-important-data
```

Install library to load env variable from file

``` bash
python -m pip install python-dotenv
```

Load the .env file. Set override=true to load it every time

``` python
from dotenv import load_dotenv

load_dotenv(override=True)  # Load environment variables from .env file
```

Use the values

``` python
GCP_PROJECT_ID = os.getenv('GCP_PROJECT_ID')
SERVICE_ACCOUNT_FILE = os.getenv('SERVICE_ACCOUNT_FILE')
STORAGE_BUCKET_NAME = os.getenv('STORAGE_BUCKET_NAME')
```

os.getenv will load the variable first from the .env file. If not found, it will check the env variable at system level.
