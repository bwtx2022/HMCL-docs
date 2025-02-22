---
title:  "稳定版更新日志"
permalink: /changelog/stable.html
date:   2021-08-22 23:18:02 +0800
categories: 更新日志
toc: true
---

<p>Notice: changelogs are written in Chinese.</p>
<h1>HMCL 3.5.3</h1>
<ul>
  <li>启动器
    <ul>
      <li>支持多人联机</li>
      <li>自动选择新添加的 Authlib-injector 服务器</li>
      <li>添加修改离线账户皮肤的功能，允许使用本地图片和 LittleSkin 等皮肤站</li>
      <li>自动检测系统内安装的 OpenJDK，包括 Liberica/Microsoft/Zulu/AdoptOpenJDK</li>
      <li>允许修改启动器字体</li>
      <li>游戏崩溃时提供崩溃分析报告</li>
      <li>添加帮助页面</li>
      <li>更换默认背景图</li>
      <li>修复微软登录页可能白屏的问题</li>
      <li>任意页面按 ESC 键可返回上一页</li>
      <li>修复启动器打开时提示找不到 DST ROOT CA X3 证书的问题</li>
      <li>修复对系统平台的识别错误导致部分平台不能正确下载 JavaFX 的问题</li>
      <li>修复 Log4j 远程代码执行漏洞</li>
    </ul>
  </li>
  <li>游戏启动
    <ul>
      <li>支持官方启动器为 Minecraft 启动参数提供的一些占位符</li>
      <li>兼容 TLauncher 游戏客户端</li>
      <li>如果在 macOS/Windows ARM 设备上使用 HMCL，HMCL 会优先使用 x86 的 JDK 运行游戏</li>
      <li>解决 Java 16 下部分 mod 不能正常运行的问题</li>
      <li>修复 Windows 下打开使用 Unicode UTF-8 提供全球语言支持选项后启动器无法打开的问题</li>
      <li>修复不能启动 BakaXL 安装后的游戏的问题</li>
      <li>修复不能正常启动 Minecraft 1.5 及以下版本的问题（需要手动删除 options.txt）</li>
    </ul>
  </li>
  <li>下载
    <ul>
      <li>启动 Minecraft 1.17 及以上版本时自动下载官方提供的 Java 16</li>
      <li>支持 CurseForge 整合包、Mod、资源包、地图 下载</li>
      <li>支持 1.17 Forge 的自动安装与游戏启动</li>
      <li>支持 1.17 下 OptiFine 与 Forge 同时安装</li>
      <li>添加模组批量更新功能</li>
      <li>添加自动选择下载源的功能</li>
      <li>允许修改默认的下载并发数</li>
    </ul>
  </li>
  <li>游戏设置
    <ul>
      <li>允许在 Java 自定义参数内覆盖启动器默认提供的启动参数，而不需要再禁止启动器生成默认参数</li>
      <li>允许在 Minecraft 自定义参数内使用 ${game_directory} 等占位符</li>
      <li>改进版本管理和游戏设置的界面</li>
      <li>添加修改游戏进程优先级的功能</li>
      <li>支持自动选择游戏内存大小</li>
      <li>添加查看模组详细介绍及打开其官方页面的功能</li>
      <li>添加 Linux 下使用系统 GLFW 及 OpenAL 的功能</li>
      <li>自定义本地库路径，允许 M1 设备运行 ARM 版本的 Minecraft</li>
      <li>添加自动选择 Java 选项，省去提示用户需要更改 Java 版本的步骤</li>
    </ul>
  </li>
  <li>整合包
    <ul>
      <li>支持使用 Fabric 作为 Mod 加载器的 CurseForge 整合包</li>
      <li>支持我的世界中文论坛整合包规范第二版，兼容 CurseForge 整合包格式，允许导入 MultiMC</li>
      <li>修复安装整合包时可能崩溃的问题</li>
      <li>修复 MCBBS 整合包实现不符合规范的问题</li>
    </ul>
  </li>
</ul>
<h1>HMCL 3.3.188</h1>
<ul>
  <li>启动器
    <ul>
      <li>修改界面</li>
      <li>更新俄语翻译</li>
      <li>改善游戏下载速度</li>
      <li>添加复制游戏实例功能</li>
      <li>支持微软正版账户登录</li>
      <li>自动设置游戏的默认语言为中文</li>
      <li>兼容 Java11+，在 Java 11+ 上运行时会自动下载 JavaFX</li>
      <li>配置文件会优先选择启动器同目录而不是工作目录</li>
      <li>支持 Authlib-injector 账户上传皮肤</li>
      <li>支持 Authlib-injector 服务器用邮箱以外的账户登录</li>
      <li>上传皮肤时自动检测 Steve、Alex 模型</li>
      <li>刷新账户时将显示进度条</li>
      <li>自定义本地库路径，允许 M1 设备运行 ARM 版本的 Minecraft</li>
      <li>启动 Minecraft 1.17 时自动下载官方提供的 Java 16</li>
      <li>允许第三方修改 HMCL 的 BMCLAPI 下载源，从而支持第三方下载源</li>
      <li>自动检测系统内安装的 OpenJDK，包括 Liberica/Microsoft/Zulu/AdoptOpenJDK</li>
      <li>修复启动 Minecraft 1.0 时不会停止等待游戏启动的问题</li>
      <li>修复首次打开整合包会弹出 3 个新建账户窗口的问题</li>
      <li>修复运行在 Java 12+ 时列表和下拉菜单不能正常显示的问题</li>
      <li>修复鼠标指针不正常的问题</li>
      <li>修复添加外置登录的正版账号后会与普通正版账号冲突的问题</li>
      <li>修复因为线程过多导致在 macOS 系统上运行崩溃的问题</li>
      <li>修复重命名游戏版本点击移动窗口而不是移动光标的问题</li>
      <li>尝试修复在游戏启动后启动器直接关闭时导致游戏卡死的问题</li>
      <li>修复启动器设置 HTTP 代理后，游戏无法访问网络的问题</li>
      <li>修复下载支持库文件失败时启动器崩溃的问题</li>
      <li>修复不能识别部分数据包的问题</li>
      <li>修复 Windows 下打开使用 Unicode UTF-8 提供全球语言支持选项后启动器无法打开的问题</li>
      <li>解决 Java 16 下部分 mod 不能正常运行的问题</li>
    </ul>
  </li>
  <li>整合包
    <ul>
      <li>更新游戏整合包后会显示新的版本号</li>
      <li>支持我的世界中文论坛整合包标准</li>
      <li>修复更新整合包下载地址不能使用在线下载自动更新整合包的问题</li>
      <li>修复服务端自动更新整合包不能更新游戏、Forge 版本的问题</li>
    </ul>
  </li>
</ul>
<h1>HMCL 3.3.172</h1>
<ul>
  <li>启动器
    <ul>
      <li>修改界面</li>
      <li>更新俄语翻译</li>
      <li>改善游戏下载速度</li>
      <li>添加复制游戏实例功能</li>
      <li>添加清理缓存文件夹按钮</li>
      <li>修改默认下载源为 MCBBS</li>
      <li>提升与 ServerSync 的兼容性</li>
      <li>添加为正版账号上传皮肤的功能</li>
      <li>支持调整并记住启动器窗口大小</li>
      <li>在日志窗口添加导出游戏日志功能</li>
      <li>现在会校验资源索引文件的完整性</li>
      <li>现在启动器代理设置对启动后的游戏有效</li>
      <li>在启动游戏、安装游戏等界面显示总下载速度</li>
      <li>游戏崩溃后显示游戏崩溃报告而不是游戏日志</li>
      <li>允许在启动游戏按钮上滑动鼠标滚轮切换游戏</li>
      <li>在删除 Mod、世界、数据包时弹出删除确认提示</li>
      <li>允许使用在启动器同目录下的 authlib-injector.jar 文件</li>
      <li>在游戏崩溃后的第二次启动时自动检查资源和支持库文件是否完整</li>
      <li>添加启动器的 JVM 参数 -Dhmcl.font.override=fontfamily 以允许 Linux 用户更换字体以解决白屏问题</li>
      <li>修复部分整合包无法修改启动时游戏窗口大小的问题</li>
      <li>修复终止游戏后启动器不会停止等待的问题</li>
      <li>修复 1.5.2 及以下版本不能下载资源文件的问题</li>
      <li>修复某些情况下启动游戏时，启动器会崩溃的问题</li>
      <li>修复进入游戏设置后无法重命名部分游戏版本的问题</li>
      <li>修复不能在 Java 17 下载 Forge 和自动更新的问题</li>
      <li>修复重命名版本时，输入不合法的新名字后的错误提示</li>
      <li>修复重命名被依赖的版本后，会破坏其他依赖这个版本的版本的问题</li>
      <li>修复在自定义游戏运行目录时，输入不合法的路径会导致崩溃的问题</li>
      <li>修复在输入特定错误的 authlib-injector 服务器地址时会导致启动器崩溃的问题</li>
    </ul>
  </li>
  <li>自动安装
    <ul>
      <li>在 OptiFine 库缺失时可以自动补全</li>
      <li>提升自动安装功能与其他启动器的兼容性</li>
      <li>在当前下载源下载失败后自动重试其他下载源</li>
      <li>在启动游戏、安装游戏等界面显示明确的安装步骤</li>
      <li>安装游戏向导内可直接切换下载源，而不需要返回启动器设置页面</li>
      <li>支持同时安装 Minecraft 1.14.4 及以上版本的 Forge 和 OptiFine</li>
      <li>自动安装页面将提示不兼容的第三方库，比如 Forge 和 Fabric 不兼容</li>
      <li>修复无法安装 Forge 1.12.2 2852 的问题</li>
      <li>修复在 Curse 整合包安装遗漏部分 Mod 的问题</li>
      <li>修复在 Curse 整合包安装部分成功时删除游戏的问题</li>
      <li>修复 1.5.2 及以下版本安装 Forge 后启动失败的问题</li>
      <li>修复从 MCBBS 下载源下载文件可能会下载到空文件的问题</li>
      <li>修复 1.12.2 同时安装 Forge, OptiFine 时无法进入游戏存档的问题</li>
    </ul>
  </li>
  <li>整合包
    <ul>
      <li>修复整合包配置丢失后整合包游戏版本不能修改配置的问题</li>
      <li>修复服务器自动更新整合包更新时可能会出现 AccessDeniedException 的问题</li>
    </ul>
  </li>
</ul>
<h1>HMCL 3.2.149</h1>
<ul>
  <li>启动器
    <ul>
      <li>改进部分错误提示</li>
      <li>更新繁体中文语言文件</li>
      <li>在主界面账户栏添加鼠标滚轮便捷切换游戏账户</li>
      <li>在主界面账户栏添加鼠标悬浮提示以查看完整游戏名</li>
      <li>修复原版游戏用熔炉图标标识的问题</li>
      <li>修复无法取消启动过程和安装过程的问题</li>
      <li>修复无法启动使用 Vivecraft 安装器新安装的游戏的问题</li>
      <li>修复启动 1.15 时不会停止等待的问题</li>
      <li>修复 Windows 下导出启动脚本对双引号的错误转义</li>
      <li>修复部分正版账号登录 1.7.10 会导致游戏崩溃的问题</li>
      <li>修复关闭 JVM 检查时仍然会检查 java.exe 是否合法的问题</li>
      <li>修复使用 BMCLAPI 不能下载 authlib-injector 和加载游戏列表的问题</li>
    </ul>
  </li>
  <li>自动安装
    <ul>
      <li>添加 MCBBS 下载源</li>
      <li>在资源索引文件不合法时尝试重新下载</li>
      <li>添加 Fabric 的 BMCLAPI 和 MCBBS 下载源支持</li>
      <li>现官方下载源下载 Forge 时依赖文件不再强制从 BMCLAPI 下载</li>
      <li>修复重复下载游戏依赖文件的问题</li>
    </ul>
  </li>
  <li>整合包
    <ul>
      <li>导出整合包时将剔除所有日志文件和 CustomSkinLoader 的缓存</li>
      <li>修复导入 HMCL 整合包时无法安装 Forge 的问题</li>
      <li>修复无法下载 Curse 整合包部分 Mod（如潘马斯）的问题</li>
      <li>修复下载 Curse 整合包 Mod 失败后会删除整合包的问题</li>
      <li>修复下载服务端整合包没有对链接转义而无法下载的问题</li>
    </ul>
  </li>
</ul>
<h1>HMCL 3.2.139</h1>
<ul>
    <li>启动器
        <ul>
            <li>添加西班牙语，更新英语、俄语翻译</li>
            <li>主页面按回车键启动游戏</li>
            <li>游戏列表内点击列表项进入游戏设置，右键列表项打开游戏管理菜单</li>
            <li>不再强制使用 java.exe</li>
            <li>日志窗口允许关闭自动滚动</li>
            <li>避免安装游戏时输入的游戏名称不符合 Windows 系统要求</li>
            <li>修复输入某些错误的 Java 路径时崩溃的问题</li>
            <li>修复浏览 Mod 列表可能出现的崩溃问题</li>
            <li>修复无法识别 Java 12、13 的问题</li>
        </ul>
    </li>
    <li>自动安装
        <ul>
            <li>添加 Fabric 自动安装</li>
            <li>新安装的游戏可以修改游戏版本</li>
            <li>修复 OptiFine 自动安装</li>
            <li>修复同时安装 Forge 和 OptiFine 自动安装失败的问题</li>
            <li>修复某些情况下无法安装 1.12.2 及以下版本的 Forge 的问题</li>
            <li>修复导出整合包导入时无法安装 1.13 Forge 和 OptiFine 的问题</li>
            <li>修复部分情况下无法下载 Forge 安装包的问题</li>
            <li>修复无法安装 1.14 和 1.15 游戏的问题</li>
        </ul>
    </li>
    <li>整合包
        <ul>
            <li>允许从给定链接下载整合包并进行安装</li>
            <li>支持导出 MultiMC 整合包</li>
            <li>修复无法下载 Curse 模组的问题</li>
            <li>修复下载 Curse 整合包失败后会删除游戏的问题</li>
        </ul>
    </li>
    <li>服主功能
        <ul>
            <li>添加 authlib-injectors.json，允许服主将添加账号页面更改为默认添加指定服务器的 Authlib Injector 账户</li>
            <li>访问 <a href="http://www.huangyuhui.net/index.php/2019/09/09/109/">http://www.huangyuhui.net/index.php/2019/09/09/109/</a> 以查看添加方法</li>
            <li>添加服务器自动更新整合包，允许服务器远程更新游戏客户端</li>
            <li>访问 <a href="http://www.huangyuhui.net/index.php/2019/11/12/118/">http://www.huangyuhui.net/index.php/2019/11/12/118/</a> 以查看添加方法</li>
        </ul>
    </li>
</ul>

<h1>HMCL 3.2.130</h1>
<ul>
  <li>启动器
    <ul>
      <li>在启动器更新时显示更新日志</li>
      <li>启动前检查是否是 Java 8~10</li>
      <li><a href="http://www.huangyuhui.net/index.php/2019/01/27/83/">支持整合包自带 Java 运行时</a></li>
      <li>在缓存目录无效时自动更改设置</li>
      <li>在登录对话框中添加注册链接</li>
      <li>将游戏依赖的动态链接库解压到 .minecraft 中而不是系统临时文件夹</li>
      <li>更新 authlib-injector</li>
    </ul>
  </li>
  <li>自动安装
    <ul>
        <li>只从 BMCLAPI 获取 Forge、OptiFine 列表</li>
        <li>添加 BMCLAPI 赞助信息</li>
        <li>支持 Forge 1.13 的自动安装</li>
        <li>支持 Forge、LiteLoader、OptiFine 的手动更新</li>
        <li>添加提示部分版本的 Forge 和 LiteLoader 不兼容的问题</li>
        <li>下载库文件失败时提供更友好的提示</li>
        <li>安装游戏时更新资源文件</li>
        <li>启动时下载缺失的 Minecraft 本体文件</li>
        <li>在安装游戏失败时删除不完全的游戏</li>
    </ul>
  </li>
  <li>游戏管理
    <ul>
      <li>支持对 Fabric 模组的管理</li>
      <li>支持数据包列表页面、模组管理面板多选</li>
      <li>添加刷新模组列表的按钮</li>
      <li>在未安装 Mod API 的情况下禁用模组管理面板</li>
      <li>忽略游戏存档名中的颜色转移符</li>
      <li>隐藏游戏版本不匹配的游戏存档</li>
      <li>添加打开存档文件夹的菜单</li>
      <li>删除在版本管理页面中的删除游戏和重命名按钮</li>
      <li>提醒用户在修改版本独立选项时需要注意游戏文件的转移</li>
      <li>支持拖拽游戏存档压缩包到游戏界面以便安装游戏存档</li>
    </ul>
  </li>
  <li>整合包
    <ul>
        <li>支持整合包拖拽到主页面打开安装向导</li>
        <li>支持新版 MultiMC 整合包的导入</li>
        <li>在更新整合包时进行游戏文件的备份</li>
        <li>从 Cursemeta 上下载 Curse 上被删除的 Mod 文件</li>
    </ul>
  </li>
  <li>修复
    <ul>
      <li>修复头像不显示头盔层的问题</li>
      <li>修复删除模组时可能导致的崩溃</li>
      <li>修复刷新数据包列表时可能的崩溃问题</li>
      <li>修复启动器皮肤预览异常的问题</li>
      <li>修复下载失败后无法删除游戏版本的问题</li>
      <li>修复刷新版本列表时的卡顿问题</li>
      <li>修复 mods 不是文件夹时无法安装模组的问题</li>
      <li>修复启动按钮无法根据背景颜色更改字体颜色的问题</li>
      <li>修复 Java 10 上 UI 错位的问题</li>
      <li>修复启动 Curse 整合包时尝试下载被禁用的模组的问题</li>
      <li>修复皮肤图片文件损坏时导致的崩溃问题</li>
      <li>修复配置文件格式不正确时导致的崩溃问题</li>
      <li>修复 Curse 整合包更新失败的问题</li>
      <li>修复自动更新弹出气泡的界面错乱问题</li>
      <li>修复下载资源文件时潜在的崩溃问题</li>
      <li>修复导入整合包时的乱码问题</li>
    </ul>
  </li>
</ul>
