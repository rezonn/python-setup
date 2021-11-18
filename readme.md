# Python 3.7.9 & TensorFlow 2.5.0 portable for Windows 10
- install [7zip](https://github.com/rezonn/python-setup)
- [Enale long paths](enable_long_path.reg)
- Download and install [Visual Studio Redistributable 2015, 2017, 2019, and 2022](https://docs.microsoft.com/ru-RU/cpp/windows/latest-supported-vc-redist?view=msvc-160#visual-studio-2015-2017-2019-and-2022)
- restart
- Download [Python 3.7.9 Windows embeddable](https://www.python.org/downloads/windows/) .
Direct link [python-3.7.9-embed-amd64.zip](https://www.python.org/ftp/python/3.7.9/python-3.7.9-embed-amd64.zip)
- Unzip to \Python folder
- Save [get-pip.py](get-pip.py) and [python37._pth](python37._pth) to \Python
- Drag get-pip.py to \Python\python.exe
- Download [termcolor-1.1.0.tar.gz](https://files.pythonhosted.org/packages/8a/48/a76be51647d0eb9f10e2a4511bf3ffb8cc1e6b14e9e4fab46173aa79f981/termcolor-1.1.0.tar.gz). Find file termcolor.py
- Copy the termcolor.py -> \Python\Lib\site-packages\
- Add \Python folder to system path
# system path
```
rundll32 sysdm.cpl,EditEnvironmentVariables
```
- System variables -> Path -> Edit -> New -> type \Python folder
- New -> type \Python\Scripts folder
# tensorflow
```
pip install tensorflow==2.5.0
```
