
Appium安装配置 
=============================

下载
------------------------------

https://bitbucket.org/appium/appium.app/downloads/

Windows Download: 下载exe可执行文件进行安装

Mac Download: 下载dmg进行安装

Mac安装
----------------------------

.. code-block:: python

    > brew install node      # get node.js
    > npm install -g appium  # get appium
    > npm install wd         # get appium client
    > appium &               # start appium
    > node your-appium-test.js

Appium Andorid环境
------------------------------

Android环境依赖于Java,  Android Sdk



Appium ios 环境
-----------------------------

Appium ios运行依赖于Xcode 


Appium Python Client
------------------------------

.. code-block:: python:

    pip install Appium-Python-Client


用法
------------------------------

.. code-block:: python

    from appium import webdriver
    from selenium import webdriver

**例子**

.. code-block:: python

    from appium import webdriver
    
    config = {
                'platformName' = 'Android',
                'platformVersion' = '6.0',
                'devicesName' = 'Android Emulator',
                'app' = '$PATH',
                'automationName' = 'Appium'
            }

    driver = webdriver.Remote('http://localhost:4723/wd/hub',config)

使用Android sdk 自带的adb命令获取devicesName

.. code-block:: java

    adb devices -l
