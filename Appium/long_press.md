
# 案例: 长按录制小视频

## 问题

长按，录制视频

## 解决办法

`
    action = TouchAction(driver)
    
    action.long_press(element,None,None,10000).perform()

`
