# 241031Mintlab

debugging
$ python get_python_api.py
-> Downloading to 'C:\Program Files (x86)\ZED SDK'
Detected platform:
         win_amd64
         Python 3.12
         ZED SDK 4.2
-> Checking if https://download.stereolabs.com/zedsdk/4.2/whl/win_amd64/pyzed-4.2-cp312-cp312-win_amd64.whl exists and is available
Traceback (most recent call last):
  File "C:\Program Files (x86)\ZED SDK\get_python_api.py", line 180, in <module>
    open(whl_file, 'wb').write(r.content)
    ^^^^^^^^^^^^^^^^^^^^
PermissionError: [Errno 13] Permission denied: 'C:\\Program Files (x86)\\ZED SDK\\pyzed-4.2-cp312-cp312-win_amd64.whl'

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "C:\Program Files (x86)\ZED SDK\get_python_api.py", line 183, in <module>
    except requests.exceptions.URLError as e:
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
AttributeError: module 'requests.exceptions' has no attribute 'URLError'. Did you mean: 'SSLError'?
