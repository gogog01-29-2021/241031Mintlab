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


https://chatgpt.com/c/67078f0e-c278-8008-93b6-b1ff575871c4








---------------------------------------------------------------------------------------------------------------------------
kimseonghyun@DESKTOP-U5TUKVJ MINGW64 /d/PlaneFill/python (main)
$ python Plane_Fill.py 
Traceback (most recent call last):
  File "D:\PlaneFill\python\Plane_Fill.py", line 3, in <module>
    from zed import ZED
  File "D:\PlaneFill\python\zed.py", line 3, in <module>
    import pyzed.sl as sl
ModuleNotFoundError: No module named 'pyzed'

kimseonghyun@DESKTOP-U5TUKVJ MINGW64 /d/PlaneFill/python (main)
$ pip install pyzed
Collecting pyzed
  Downloading pyzed-1.3.0-py3-none-any.whl.metadata (235 bytes)
Collecting durationpy (from pyzed)
  Downloading durationpy-0.9-py3-none-any.whl.metadata (338 bytes)
Requirement already satisfied: python-dateutil in c:\users\kimseonghyun\anaconda3\lib\site-packages (from pyzed) (2.9.0.post0)
Requirement already satisfied: requests in c:\users\kimseonghyun\anaconda3\lib\site-packages (from pyzed) (2.32.2)
Requirement already satisfied: six>=1.5 in c:\users\kimseonghyun\anaconda3\lib\site-packages (from python-dateutil->pyzed) (1.16.0)
Requirement already satisfied: charset-normalizer<4,>=2 in c:\users\kimseonghyun\anaconda3\lib\site-packages (from requests->pyzed) (2.0.4)
Requirement already satisfied: idna<4,>=2.5 in c:\users\kimseonghyun\anaconda3\lib\site-packages (from requests->pyzed) (3.7)
Requirement already satisfied: urllib3<3,>=1.21.1 in c:\users\kimseonghyun\anaconda3\lib\site-packages (from requests->pyzed) (2.2.2)
Requirement already satisfied: certifi>=2017.4.17 in c:\users\kimseonghyun\anaconda3\lib\site-packages (from requests->pyzed) (2024.8.30)
Downloading pyzed-1.3.0-py3-none-any.whl (3.1 kB)
Downloading durationpy-0.9-py3-none-any.whl (3.5 kB)
Installing collected packages: durationpy, pyzed
Successfully installed durationpy-0.9 pyzed-1.3.0

kimseonghyun@DESKTOP-U5TUKVJ MINGW64 /d/PlaneFill/python (main)
$ python Plane_Fill.py 
Traceback (most recent call last):
  File "D:\PlaneFill\python\Plane_Fill.py", line 3, in <module>
    from zed import ZED
  File "D:\PlaneFill\python\zed.py", line 3, in <module>
    import pyzed.sl as sl
ModuleNotFoundError: No module named 'pyzed.sl'; 'pyzed' is not a package  





