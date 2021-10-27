# Python 3.7.9 portable for Windows 10
- [Enale long paths](enable_long_path.reg) , restart
- Download [Python 3.7.9 Windows embeddable](https://www.python.org/downloads/windows/) .
Direct link [python-3.7.9-embed-amd64.zip](https://www.python.org/ftp/python/3.7.9/python-3.7.9-embed-amd64.zip)
- Unpack it to D:/python
- Modify D:/python/python*.pth. Find line
```
.
# Uncomment to run site.main() automatically
#import site
```
replace to
```
.
.\Lib\site-packages\
import site
```


- [get-pip.py](get-pip.py)
- Move it to D:/python
- Drag get-pip.py to python.exe

## Pip install ..
Example
```
d:
chdir "D:\Python\Scripts"
pip.exe install gym
pip install tensorflow

pause
```
## Python ..
```
D:/python/python.exe helloworld.py
```
