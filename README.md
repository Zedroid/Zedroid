# Zedroid-
Xedroid
https://github.com/alystair/my-productivity-stack/blob/master/Launch%20Calculator.ahk

https://www.sevenforums.com/general-discussion/35682-disable-shift-click-taskbar.html#

    +LButton::                      ;  Shift + LButton hotkey.

    MouseGetPos,,, win          ; Get window under mouse.

    ; If this window is the taskbar,  mode:="", otherwise mode:="{Blind}".

   
     mode :=  WinExist("ahk_class Shell_TrayWnd ahk_id " win) ? "" : "{Blind}"

     Send %mode%{LButton Down}   ; Click  down, filtering out Shift if mode="".

    KeyWait LButton              ; Wait for button to be  physically released.

    Send %mode%{LButton Up}     ; Click up.

    return
