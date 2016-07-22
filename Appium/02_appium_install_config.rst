
Appium安装配置 
=============================

下载
------------------------------

https://bitbucket.org/appium/appium.app/downloads/

Windows Download:

Mac Download:

Mac安装
----------------------------

.. code-block:: python

    > brew install node      # get node.js
    > npm install -g appium  # get appium
    > npm install wd         # get appium client
    > appium &               # start appium
    > node your-appium-test.js

Andorid environmnet
------------------------------

Java,  Android Sdk



ios environment
-----------------------------

Xcode 


Appium Python Client
------------------------------

.. code-block:: python:

    pip install Appium-Python-Client


Usage
------------------------------

.. code-block:: python

    from appium import webdriver
    from selenium import webdriver

**example**

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
