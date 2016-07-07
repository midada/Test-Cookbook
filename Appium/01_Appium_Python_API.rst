

Appium Python Api
==========================

Api : 应用安装、删除
-------------------------

1.检查应用是否已经安装

    driver.is_app_installed("com.packagename")

2.应用安装

    driver.install_app('/path/com.packagename.apk')

3.卸载应用

    driver.remove_app('com.packagename.apk')


