> _[中文說明在文章後面](https://github.com/howar31/Trove-AHK-AutoFish#trove-ahk-autofish-1)_

# Trove-AHK-AutoFish
This is an AutoHotKey script for auto fishing in Trove.

Latest update: 2015/08/10

# Feature
* Using **Memory Address** to detect biting.
> Very solid compare to image search or audio detect method.

* Auto fishing in background
> As long as you have sufficient lure, this script can run in the background and automatically fishing for you without interfearence your current work.  That is, you can use your computer while Trove fishing in the background.

* Toggleable **Auto Boot Throw (ABT)** mechanism.
> Automatically discard the _Old Boot_ from your backpack.  Convenient for long-time fishing.
> 
> Press **F9** to toggle ABT on or off. Turning off the ABT mechanism to make sure AHK won't move your mouse.  Sometimes AHK ImageSearch will mis-find the image and accidentally move your mouse.  It's better to turn ABT off if you are currently working on other windows and have Trove minimized in the background.
>
> ABT is always available even when you're not auto fishing.  You may press **F9** at any time to clean up your backpack.

* Toggleable **Information Tooltip**
> Hotkeys instruction and fishing info are always available in tooltop.
>
> Press **F8** to toggle showing or hiding the info tooltip.

# Installation
1. Download and install AutoHotKey from the [official website](http://www.autohotkey.com/).
> AutoHotKey main program is needed to run the .ahk file.  Running .ahk script file other than the compiled .exe file to make sure that the script is cleanp and pure without any unintended modification.

2. Download files from this repo.
> You may find the **Download ZIP** button on the repo page.  Extract the .zip file and you can find the files below.
 * **TroveAutoFish.ahk**
 > This is the main AHK script file.

 * **boot.bmp**
 > This is the image used for ImageSearch by AHK to find the boot in your backpack.  You may make your own screenshot of _Old Boot_ if the auto boot throw is not working.

3. Put the boot.bmp file under C:\  (C:\boot.bmp)
 > This path is currently hard-coded in AHK script.  So if you want to change the path you may modify the script yourself.

# Usage
1. Double click script file **TroveAutoFish.ahk** to execute the script.
> A _green H_ icon will show up when the script is running.  If you can not execute the script, make sure you have AutoHotKey correctlly installed.

2. Open **Trove**, find a pool, press **B** to open your backpack, and press **F11** to start auto fishing.
> Open your backpack to prevent camera rotate while moving mouse.  And also allow AHK ImageSearch to find the Old Boot in your backpack.

3. The default of auto boot throw (ABT) is off at start.  Press **F9** to toggle on.
> Note that you have to keep Trove window active for AHK ImageSearch.  And AHK will use and move your mouse to throw the boot out of your backpack once if found the match image.
>
> If ABT is not working correctly, you may:
>
> 1. Item will rotate while mouse hover on them.  Close then reopen the backpack will set the item to default position which will match the boot.bmp
> 2. Create a new boot.bmp by yourself.  Just simply take a screenshot of the _Old Boot_.  Note that, hover will rotate the item.  You don't want a rotated image which will cause the ImageSearch fail.

4. Press **F10** to stop and terminate the whole script.

Hotkeys and fishing info are also displayed as tooltip.

--

# Trove-AHK-AutoFish
這是 Trove 自動釣魚的 AutoHotKey 腳本。

最新更新: 2015/08/10

# 特色
* 使用 **記憶體位置** 偵測是否有魚上鉤
> 使用記憶體偵測的方式非常精準，比圖片比對或聲音偵測的釣魚方式還要更好。

* 背景自動釣魚
> 只要背包裡的魚餌充足，這個腳本可以完全不影響你使用電腦，自動在背景釣魚，也就是說，你可以把 Trove 縮小在工作列釣魚，然後用電腦做其他事情。

* 可切換開關的 **自動丟鞋 (ABT)** 機制
> 腳本可以自動的把背包內的 _鞋子 (Old Boot)_ 丟掉，有利於長時間自動釣魚。
> 
> 按 **F9** 可切換自動丟鞋功能的開關，將 自動丟鞋 (ABT) 功能關閉時，可以確保 AHK 完全不會動到你的滑鼠。有時候 AHK 的圖片搜尋功能會比對錯誤，因此讓滑鼠亂飄，如果你將 Trove 縮小到工具列背景釣魚，同時用電腦進行其他工作，建議將丟鞋功能關閉以確保滑鼠不會亂動。
>
> 自動丟鞋隨時可用，沒有自動釣魚的時候也可以按 **F9** 清理背包。

* 可切換顯示的 **資訊浮動視窗**
> 隨時提示按鍵功能以及釣魚相關資訊。
>
> 可按 **F8** 切換顯示或隱藏浮動視窗。

# 安裝說明
1. 到 AutoHotKey [官方網站](http://www.autohotkey.com/) 下載並安裝程式
> 你必需要安裝 AutoHotKey 程式才能執行 .ahk 檔案。推薦執行 .ahk 腳本檔案而非製作完成的 .exe 檔案，以確保腳本完全乾淨無毒，不會遭人加料修改。

2. 在這個頁面下載檔案
> 在網頁右邊可以找到 **Download ZIP** 的按鈕，下載並解壓縮 .zip 檔案即可找到下列檔案。
 * **TroveAutoFish.ahk**
 > 這是主要的 AHK 腳本檔案。

 * **boot.bmp**
 > 這是一張鞋子的圖片，用來讓 AHK 進行圖片比對搜尋背包內的鞋子用。若腳本的自動丟鞋功能無法正常運作，你也可以自行拍照截圖鞋子的圖片來取代這個檔案。

3. 把 boot.bmp 放在 C:\ 目錄底下  (C:\boot.bmp)
 > 這個路徑位置目前是寫死在腳本內的，所以如果你想把圖片放在其他路徑你可以自行修改腳本內的路徑位置。

# 使用方式
1. 點兩下 **TroveAutoFish.ahk** 開始執行腳本
> 當腳本執行時工具列會出現一個 _綠底的H_ 圖示。如果你點兩下無法執行腳本，請確定 AutoHotKey 是否有正確安裝。

2. 開啟 **Trove** ，然後找個魚池，按 **B** 打開背包，再按 **F11** 即可開始自動釣魚
> 打開背包是為了防止滑鼠轉動視角而無法對準魚池拋竿，並讓 AHK 的圖片比對能搜尋背包內的鞋子。

3. 自動丟鞋功能 (ABT) 剛啟動時預設是關閉的，按 **F9** 可切換開啟
> 注意，你必需要保持 Trove 視窗為啟用狀態，這樣腳本才能進行圖片比對搜尋。每當 AHK 發現符合的圖片時，會自動移動你的滑鼠把鞋子丟掉。
>
> 如果 ABT 無法正常運作，你可以嘗試:
>
> 1. 當滑鼠指在物品上的時候物品會旋轉，把背包關掉然後重新打開可以讓物品回到原始位置，也就是 boot.bmp 預設的位置。
> 2. 自己重新建立一個新的 boot.bmp 檔案，只要將 _Old Boot_ 拍照截圖儲存即可，注意滑鼠指在物品上的時候會旋轉，旋轉過的物品截圖會造成圖片比對搜尋失敗而無法正常運作。

4. 按 **F10** 停止並完全關閉整個腳本

按鍵功能與相關資訊也可參考腳本的資訊浮動視窗。