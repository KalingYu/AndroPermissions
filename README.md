# AndroPermissions
This is a tool for checking permissions in Android APK, which extracted from [Androguard]("https://github.com/androguard/androguard"). And we contribute some feature differented from Androguard.

1. Put the tool into Windows plantform, while the Androguard is just fit for Linux (it's difficult to install in Win).
2. Figure out the MultiDex problem. The Androguard just can handle with the APK with only one .dex.
3. Output the txt file and filter the Dangerous and Signature permissions.

## Usage
This tool can work well in Win, Mac and Linux.

1. You need [Python 2.7.x]("https://www.python.org/") and install the [setuptools]("https://pypi.python.org/pypi/setuptools"), which are found in the official website.
2. Copy AndroPermissions into local, and excute following code in terminal:
  ```python
  python setup.py install
  ```
3. Then given the APK for analyzing and excute:
  ```python
  androlyze.py -i "TestActivity.py" -x
  ```
  The TestActivity.apk is the demo for checking permissions.
4. Final, you will get the two txt files for permissions results.
