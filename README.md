# Personal File Master
PFM: Personal(P.o-r.n) File Manager for Windows
v0.1 2021-06
Please use it at your own RISK!
http://www.pfilemaster.com

mailto:pfilemaster@gmail.com for any suggestions.

Personal (P actually for P-orn) file master
Introduction to existing functions:
* Manage multiple hard disk devices for personal hobby videos, automatically scan files, and store as many as 100,000 files
* The identification of the device will not be affected by the change of the drive letter
* Built-in video player supports playing most video formats
* Esc key to quickly close all pictures/play
* Support additional memo, mark
* Automatically obtain file media information in batches (such as resolution/bitrate/decoder, etc.)
* Special recommendation: multi-keyword quick search database, title sorting, such as "abp 30"
* Special recommendation: batch analysis file number/code
* Special recommendation: Generate preview images in batches (PNG or GIF: make the preview animation)
* Special recommendation: batch download (scraping) video information: cover/title/starring, etc.
* Special recommendation: Wall play mode, play four files at the same time, control the progress with one-handed keyboard, and load/save the profile
* Special recommendation: Find duplicate files according to the checksum and allow batch deletion
* Special recommendation: Monitor a certain directory and automatically analyze the newly downloaded .torrent file, and give a warning if it may have been downloaded
* Find the record with the same number/code for easy selection (for deletion)
* Batch generation of KODI .nfo files (not fully tested)
* Check whether files still exist in batches/copy files
* Delete records/files in batch
* Batch set multiple fields 
* Export file name list
* Automatic database backup
* Multi-language (not perfect, under development)
* Scraping supports custom Python scripts

=== More features are under development (only plans, due to time and ability may not be able to complete) ===
* More complete tagging/scoring system
* Automatic translation of content
* Perfect multi-language system: labeling/translation/scraping
* Batch storage with automatic sub-directory renamed
* Rename support scripting/RegEx
* Import data from .nfo to prevent database loss
* More powerful filter condition selecting
* The wall play randomly selects videos based on hobbies
* Support DVD/Bluray registration (such as recording physical butterfly racks) and NAS devices
* Automatically update version
* Support download/upload of Google drive/mega/Baidu disk
* Multiple favorite parts of the video/advertisements and other categories can be defined, and the player automatically jumps to
* Support VLC embedding
* Support file split/merge/re-encode
* Download monitoring, automatically suggest storage devices and directories based on tags
* Boss key
* User login password
* Database encryption and export
* Support for video/torrent publishers: Need feedback function (thank you)

Dear AV film enthusiasts, I've wanted to write this software for a long time. I haven't found any similar useful specialized software on the market, so I wrote the first version of v0.1 on the premise that the recent project is less stressful and private time.
I will continue to develop in my free time in the future, but please forgive me. This software is only developed based on my personal hobbies. Although I want to realize my own ideas and the ideas of its fans as much as possible, I may not be able to fully satisfy them due to insufficient time and my own development capabilities. Nor can it guarantee that subsequent versions are fully compatible with the existing ones and preserve the data (but I will try to provide a smooth upgrade method).

May the world be peaceful, the Pandemic will disappear, and all AV enthusiasts may find their favorites and live happily.

Here is a serious statement: I am not afraid of offending, I am opposed to all child pornography. I have not added any restriction or destruction logic by now, but I might do something in the future versions, in a polite way.

=====
v0.1
The easiest way to use:

1. Unzip/unrar and run PFMaster.exe

2. The initial use will pop up the preference interface, select the UI language and save config, currently only ENG/CHS two languages are used, and it will be added later.

3. The first time you use it, the Device Manager will pop up and ask to add at least one storage device, plug in your AV storage hard disk, and select it in the "Select a device" dialog box.

4. Then you will be asked to add a directory of the device immediately. This directory should only be the directory that saves all your AV videos, such as "AV" or "Action Movies". Of course, you can select the root directory. Need more scan time and may be detrimental to future functions.

5. Then PFM will start to scan the files. The process may be long, but it is allowed to cancel and continue next time without dup adding.

6. After adding all the devices and directories, close the device manager, you can use the basic functions in the main interface, such as editing, double-clicking to play, searching, etc. In the searching box, you can enter multiple keywords separated by spaces. For example, if you want to find abp-030, you should enter "abp 30". The records containing these keywords will be filtered and displayed. If the scraping is completed, you can enter actors such as "SNIS RION".

7. Generally, we still need a few more steps to complete the basic work, but PFM has tried to make it simple and batched. The first is the analysis number/code. You can select Batch Op (F6) in the main interface or the file list of the device manager, and select "Auto analysis code". At present, only Japanese videos are better recognized, but I still don't have free time to deal with such as FC2/1pondo, etc. I have relatively few Western videos and have not implemented processing, but I will continue to implement them later. and implement an open script solution.

8. Then we can "Get video info/scrape" in the same interface and select the scraper to run. The main purpose of the scraper is to download basic information such as title/manufacturer/performer(s)/cover file, etc. according to the number/code. I have implemented two website scrapers and an example of an external Python script scraper is far from enough, but for my personal use, it is still reluctant.

9. Next is to generate the preview image, "Media information" in the batch operation interface, this step can be in no particular order with the above two steps, it is mainly to generate the basic information of the video file such as duration/resolution/preview Picture, PFM has done a lot of work in generating preview pictures. It can generate the traditional PNG palace format, and I think it is good but the GIF animation picture is very slow, which divided the video into N segments (scenes) and generated thumbnails. The process can be done for a long time, you can quit halfway and start again next time, just choose not to overwrite.

10. Finally, I will give a brief introduction to the wall play function, which you know when to use :>. Currently, 4 videos are allowed to be played at the same time. You can click the window or press Enter to specify the video one by one, and then press the space to play together.  One hand with keyboard (note that you must not use input method) to complete all operations, such as 1-4 or F1-F4 to select screen, arrow keys to fast forward and rewind, F5-F12, <,>, ~ all have special functions. Just try to press every key and see what happens. The most important thing is to press Esc to immediately close the playback. You can save the profile and reload it next time. The random function is not completed. In the future, it is planned to automatically jump to the defined favorite part. It is recommended to convert to a lower resolution such as 720p if you are running out of CPU. PFM should support the conversion video function in the future.

11. There are also some others functions that I think are pretty good, such as finding duplicate files (it is usually exactly the same according to the size and checksum) or files with the same number/code, batch selection then delete can save space. Another thing is monitoring .torrent files, It automatically analyzes the number/code and looks it up. If there is a record or more, it will remind you that you may have downloaded it before,  Of course this is just a reminder. I myself often download duplicate videos, wasting time and hard disk. Note: Deleting files is just throwing in the recycle bin and not really delete them, and there is still a chance to restore it by yourself. Please don't blame me if you want to get it back after emptying the recycle bin.

12. More features are coming, but I also have to work to make a living, so I can't devote myself to this stuff. I'll do my best. 

PFM Author Edward. 2021-06-15
pfilemaster@gmail.com

=== 简体中文 ===
AV文件大师
现有功能简介：
* 管理个人爱好视频的多个硬盘设备，自动扫描文件，10万级文件数量存储量
* 不会受盘符改变影响设备的辨认
* 内置播放器, 支持播放大部分视频格式
* 可外部运行其他播放器播放
* Esc键快速关闭所有图片/播放
* 支持额外文件备注，自我评分
* 批量自动获取文件媒体信息（例如分辨率/码率/解码器等）
* 特别推荐：多关键字快速查找数据库、标题排序，例如 "abp  30"
* 特别推荐：批量分析文件番号
* 特别推荐：批量产生预览图片（PNG或动图GIF：让预览动起来）
* 特别推荐：批量下载（刮削）影片信息：封面/标题/主演等
* 特别推荐：播放墙，四个文件一起播放，单手键盘掌控进度，可存储配置
* 特别推荐：根据校验码查找重复的文件，允许批量删除
* 特别推荐：监控某目录自动分析新下载的.torrent种子文件，如果可能已经下载则给出警告
* 查找同番号记录以便取舍
* 批量产生KODI .nfo文件
* 批量查找文件是否仍存在/复制文件
* 批量删除文件记录
* 批量设置文件多个属性
* 导出文件名列表
* 自动备份数据库
* 多语言（未完善，开发中）
* 刮削支持自定义Python脚本

=== 更多功能计划开发中（只是计划，由于时间和能力未必能完成） ===
* 较完善的标签/评分系统
* 内容自动翻译
* 完善的多语言系统：标签/翻译/刮削
* 批量自动分目录改名存储
* 改名脚本插件/RegEx
* 从.nfo导入数据，防止数据库丢失
* 更强大的过滤条件功能
* 播放墙根据爱好随机选片
* 支持DVD/Bluray登记（例如记录物理蝶架）和NAS设备
* 自动更新版本
* 支持Google drive/mega/百度盘/阿里云盘的下载/上传
* 可定义视频多个精彩部分/无用广告等类别，播放器自动跳跃
* 支持VLC嵌入
* 支持文件分割/合并/重编码
* 下载监控，自动根据标签建议存储设备和目录
* 老板键
* 用户登录密码
* 数据库加密、导出
* 对影片/种子发布者的支持：需要反馈功能（谢谢)

各位AV影片爱好者，我想写这个软件很久了，市场上一直没发现类似的好用的专门软件，于是在最近项目没那么紧张有点私人时间的前提下写了一个初版v0.1，
后续我会继续空闲时间开发，但请各位原谅，此软件仅仅是基于个人爱好开发，我虽然想尽量实现自己和各爱好者的想法，但是由于时间和自身开发能力不足，未必能全部满足，
也不能保证后续的版本跟现有的完全兼容而保全数据（但是我会尽量提供平滑的升级方法）。

愿天下太平，愿疫情消失，愿各AV爱好者找到自己的最爱并且生活开心写意。

在此严肃声明：不怕得罪，我反对一切的儿童色情，我目前没有加入任何限制或破坏逻辑，但不保证以后的版本不会加以限制（但也不会刻意破坏）。

=====
v0.1
最简单使用方法:

1. 解压运行PFMaster.exe

2. 初始使用会弹出配置界面, 选定界面语言保存配置, 目前只搞了ENG/CHS两种语言,迟点增加.

3. 初次使用会弹出设备管理器要求至少新增一个存储设备, 插好你的存储AV的硬盘, 在新增设备对话框中选择它.

4. 然后马上会要求你增加一个该设备下的目录, 该目录应该只是保存所有你的AV视频的目录, 例如"AV"或者"动作片", 当然也可以直接选择根目录, 查找费多点时间且可能对以后的功能不利.

5. 然后PFM会开始扫描文件, 该过程可能较长, 但是允许中途取消并下次继续, 不会重复添加.

6. 在增加完所有设备和目录后, 关闭设备管理器, 你可以在主界面中使用基本的功能了, 例如编辑双击播放, 查找等, 如果是查找, 可以输入多个关键字用空格分隔, 例如你想找 abp-030, 应该输入"abp 30", 包含这些关键字的记录会过滤显示出来, 如果刮削完成后, 可以输入演员例如"SNIS RION"之类的.

7. 一般地, 我们还需要几步才能完成基础工作, 但是PFM已经尽量让其简单和批量化, 首先是分析番号, 可以在主界面或者设备管理器的文件清单选择批量处理(F6), 选择"自动分析番号", 目前只对日本片的通用番号进行比较好的辨识, 但是诸如FC2/1pondo等我还没时间处理好, 西片我本人比较少也没实现处理, 迟些我会陆续实现并给出开放的脚本解决方案.

8. 然后我们可以同样的界面进行"刮削视频信息", 选择刮削器运行, 刮削器主要目的是根据番号去其他现成网站下载基本信息如标题/厂商/主演/封面等, 我目前实现了两个固定刮削器和一个外部脚本刮削器例子, 还远远不够, 但是对于我个人使用还算勉强的.

9. 再之后就是生成预览图, 同一样是批处理界面的"媒体信息"部分, 这一步骤跟上面两步可以不分先后, 它主要是生成视频文件的基本信息例如时长/分辨率/预览图, 其中预览图PFM做了比较多的工作, 目前可以生成传统的PNG宫格式预览图, 还有我觉得不错但是巨慢的GIF动图, 都是按照平均切分N段(场景)然后生成预览图的逻辑. 该过程可以搞好久, 可以中途退出下次再重来, 选择不覆盖就行.

10. 最后简介一下播放墙功能, 用来干什么我就不明说了, 目前允许4个视频同时播, 可以逐个鼠标点击窗口或者回车指定视频, 然后按空格就一起播, 过程中完全可以一只手按键盘(注意要输入英文状态)完成所有操作, 例如1-4或者F1-F4能选哪个屏, 方向键快进快退, F5-F12,<,>,~都有特殊功能,可以什么键都按一下看有什么反应, 最重要按Esc马上关闭播放. 还能保存方案下次调出, 随机功能未完成, 以后还打算做成自动跳到定义好的精彩部分. 目前建议如果播放4个视频你的机器比较吃力, 建议转换为低一点分辨率的例如720p, 以后PFM应该会支持转换视频功能.

11. 还有一些我觉得不错的功能例如查找重复的文件(根据大小和校验码找出来一般就是一模一样的)或者番号一样的文件, 批量选择删除可以节省空间, 另外例如监控.torrent种子文件, 自动分析出番号然后查找, 如果有记录会提醒你可能以前下载过, 不过当然这只是提醒, 我自己就经常下载了重复的视频, 浪费时间和硬盘. 注意: 删除文件只是投入了回收站并非正在删除, 还有机会自己恢复回去, 清空回收站后再想找回来就不要怨我.

12. 更多的功能更新中, 不过我也要工作吃饭, 所以不能全心投入搞这玩意, 尽力而为吧.

=== 繁體中文 ===
AV文件大師
現有功能簡介：
* 管理個人愛好視頻的多個硬碟設備，自動掃描檔，10萬級檔數量存儲量
* 不會受盤符改變影響設備的辨認
* 內置播放機, 支援播放大部分視頻格式
* 可外部運行其他播放機播放
* Esc鍵快速關閉所有圖片/播放
* 支援額外檔備註，自我評分
* 批量自動獲取檔媒體資訊（例如解析度/碼率/解碼器等）
* 特別推薦：多關鍵字快速查找資料庫、標題排序，例如 "abp  30"
* 特別推薦：批量分析檔番號
* 特別推薦：批量產生預覽圖片（PNG或動圖GIF：讓預覽動起來）
* 特別推薦：批量下載（刮削）影片資訊：封面/標題/主演等
* 特別推薦：播放牆，四個檔一起播放，單手鍵盤掌控進度，可存儲配置
* 特別推薦：根據校驗碼查找重複的檔，允許批量刪除
* 特別推薦：監控某目錄自動分析新下載的.torrent種子檔，如果可能已經下載則給出警告
* 查找同番號記錄以便取捨
* 批量產生KODI .nfo文件
* 批量查找檔是否仍存在/複製檔
* 批量刪除檔記錄
* 批量設置檔多個屬性
* 匯出檔案名列表
* 自動備份資料庫
* 多語言（未完善，開發中）
* 刮削支持自訂Python腳本

=== 更多功能計畫開發中（只是計畫，由於時間和能力未必能完成） ===
* 較完善的標籤/評分系統
* 內容自動翻譯
* 完善的多語言系統：標籤/翻譯/刮削
* 批量自動分目錄改名存儲
* 改名腳本外掛程式/RegEx
* 從.nfo導入資料，防止資料庫丟失
* 更強大的過濾條件功能
* 播放牆根據愛好隨機選片
* 支援DVD/Bluray登記（例如記錄物理蝶架）和NAS設備
* 自動更新版本
* 支持Google drive/mega/百度盤/阿裡雲盤的下載/上傳
* 可定義視頻多個精彩部分/無用廣告等類別，播放機自動跳躍
* 支持VLC嵌入
* 支援檔分割/合併/重編碼
* 下載監控，自動根據標籤建議存放裝置和目錄
* 老闆鍵
* 使用者登錄密碼
* 資料庫加密、匯出
* 對影片/種子發佈者的支持：需要回饋功能（謝謝)

各位AV影片愛好者，我想寫這個軟體很久了，市場上一直沒發現類似的好用的專門軟體，於是在最近專案沒那麼緊張有點私人時間的前提下寫了一個初版v0.1，
後續我會繼續閒置時間開發，但請各位原諒，此軟體僅僅是基於個人愛好開發，我雖然想儘量實現自己和各愛好者的想法，但是由於時間和自身開發能力不足，未必能全部滿足，
也不能保證後續的版本跟現有的完全相容而保全資料（但是我會儘量提供平滑的升級方法）。

願天下太平，願疫情消失，願各AV愛好者找到自己的最愛並且生活開心寫意。

在此嚴肅聲明：不怕得罪，我反對一切的兒童色情，我目前沒有加入任何限制或破壞邏輯，但不保證以後的版本不會加以限制（但也不會刻意破壞）。

=====
v0.1
最簡單使用方法:

1. 解壓運行PFMaster.exe

2. 初始使用會彈出配置介面, 選定介面語言保存配置, 目前只搞了ENG/CHS兩種語言,遲點增加.

3. 初次使用會彈出裝置管理員要求至少新增一個存放裝置, 插好你的存儲AV的硬碟, 在新增設備對話方塊中選擇它.

4. 然後馬上會要求你增加一個該設備下的目錄, 該目錄應該只是保存所有你的AV視頻的目錄, 例如"AV"或者"動作片", 當然也可以直接選擇根目錄, 查找費多點時間且可能對以後的功能不利.

5. 然後PFM會開始掃描檔, 該過程可能較長, 但是允許中途取消並下次繼續, 不會重複添加.

6. 在增加完所有設備和目錄後, 關閉裝置管理員, 你可以在主介面中使用基本的功能了, 例如編輯按兩下播放, 查找等, 如果是查找, 可以輸入多個關鍵字用空格分隔, 例如你想找 abp-030, 應該輸入"abp 30", 包含這些關鍵字的記錄會過濾顯示出來, 如果刮削完成後, 可以輸入演員例如"SNIS RION"之類的.

7. 一般地, 我們還需要幾步才能完成基礎工作, 但是PFM已經儘量讓其簡單和批量化, 首先是分析番號, 可以在主介面或者裝置管理員的檔清單選擇批量處理(F6), 選擇"自動分析番號", 目前只對日本片的通用番號進行比較好的辨識, 但是諸如FC2/1pondo等我還沒時間處理好, 西片我本人比較少也沒實現處理, 遲些我會陸續實現並給出開放的腳本解決方案.

8. 然後我們可以同樣的介面進行"刮削視頻資訊", 選擇刮削器運行, 刮削器主要目的是根據番號去其他現成網站下載基本資訊如標題/廠商/主演/封面等, 我目前實現了兩個固定刮削器和一個外部腳本刮削器例子, 還遠遠不夠, 但是對於我個人使用還算勉強的.

9. 再之後就是生成預覽圖, 同一樣是批次處理介面的"媒體資訊"部分, 這一步驟跟上面兩步可以不分先後, 它主要是生成視頻檔的基本資訊例如時長/解析度/預覽圖, 其中預覽圖PFM做了比較多的工作, 目前可以生成傳統的PNG宮格式預覽圖, 還有我覺得不錯但是巨慢的GIF動圖, 都是按照平均切分N段(場景)然後生成預覽圖的邏輯. 該過程可以搞好久, 可以中途退出下次再重來, 選擇不覆蓋就行.

10. 最後簡介一下播放牆功能, 用來幹什麼我就不明說了, 目前允許4個視頻同時播, 可以逐個滑鼠點擊視窗或者回車指定視頻, 然後按空格就一起播, 過程中完全可以一隻手按鍵盤(注意要輸入英文狀態)完成所有操作, 例如1-4或者F1-F4能選哪個屏, 方向鍵快進快退, F5-F12,<,>,~都有特殊功能,可以什麼鍵都按一下看有什麼反應, 最重要按Esc馬上關閉播放. 還能保存方案下次調出, 隨機功能未完成, 以後還打算做成自動跳到定義好的精彩部分. 目前建議如果播放4個視頻你的機器比較吃力, 建議轉換為低一點解析度的例如720p, 以後PFM應該會支援轉換視頻功能.

11. 還有一些我覺得不錯的功能例如查找重複的檔(根據大小和校驗碼找出來一般就是一模一樣的)或者番號一樣的檔, 批量選擇刪除可以節省空間, 另外例如監控.torrent種子檔, 自動分析出番號然後查找, 如果有記錄會提醒你可能以前下載過, 不過當然這只是提醒, 我自己就經常下載了重複的視頻, 浪費時間和硬碟. 注意: 刪除檔只是投入了回收站並非正在刪除, 還有機會自己恢復回去, 清空回收站後再想找回來就不要怨我.

12. 更多的功能更新中, 不過我也要工作吃飯, 所以不能全心投入搞這玩意, 盡力而為吧.

