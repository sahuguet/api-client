# Gro API Client
  
## Set up the environment
```
cd ~/gro
git clone https://github.com/gro-intelligence/api-client.git
export PYTHONPATH=~/gro/api-client:$PYTHONPATH
```
To avoid typing your password on the command line, you can get an API access token as follows:
```
cd ~/gro/api/client
python gro_client.py --user_email=... --user_password=.... --print_token
```
To save it in a bash environment variable:                                               
```
export GROAPI_TOKEN=`python gro_client.py --user_email=... --user_password=... --print_token`
```
For repeated use, you may want to save PYTHONPATH and GROAPI_TOKEN as permanent environment variables in your bash_profile (or equivalent).
## Examples
Try [quick_start.py](api/client/samples/quick_start.py):
```
cd ~/gro/api/client/samples/
python quick_start.py
```
A more advanced example is [sugar.py](api/client/samples/crop_models/sugar.py):
```
cd ~/gro/api/client/samples/crop_models/
python sugar.py
```
Further documentation can be found in the [api/client/](api/client) directory.
