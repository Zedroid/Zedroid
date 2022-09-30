# Zedroid-
Xedroid
https://github.com/wisehackermonkey/ultimate-tts-reader
https://github.com/alystair/my-productivity-stack/blob/master/Launch%20Calculator.ahk
https://github.com/sayyid5416/Links-Extractor
https://github.com/clechasseur/pathcopycopy
Pytranscriber
Mpv https://github.com/stax76/mpv.net/issues/488
Wizmouse

autostart ahk
https://github.com/AutoHotkey/Ahk2Exe add shortcut to startup folder
FileCreateShortcut, %A_ScriptFullPath%, %A_Startup%\shortcutname.lnk



https://www.sevenforums.com/general-discussion/35682-disable-shift-click-taskbar.html#

    +LButton::                      ;  Shift + LButton hotkey.

    MouseGetPos,,, win          ; Get window under mouse.

    ; If this window is the taskbar,  mode:="", otherwise mode:="{Blind}".

   
     mode :=  WinExist("ahk_class Shell_TrayWnd ahk_id " win) ? "" : "{Blind}"

     Send %mode%{LButton Down}   ; Click  down, filtering out Shift if mode="".

    KeyWait LButton              ; Wait for button to be  physically released.

    Send %mode%{LButton Up}     ; Click up.

    return

Frederik LongReplied on January 30, 2021
How can I move folders from an old computer to a new computer so that I retain the same "Date Modified"?

Try this:

Create a desktop shortcut for cmd.exe.

https://github.com/raszpl/hackahackernews


Double-click this shortcut. You will get a black frame.
Type this command and press Enter:
robocopy  "H:\FolderName"  "C:\Users\David\FolderName"  /e  /w:1  /r:1


robocopy <"source"> <"destination">  /e  /w:1  /r:1
https://answers.microsoft.com/en-us/windows/forum/all/retaining-the-original-date-modified-of-folders/0c0982f9-03a5-47f6-ae32-f2691d647889

https://github.com/marzzzello/mpv_thumbnail_script/issues/22#issuecomment-1179770239

