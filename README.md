# V2ray for Doprax 超群收藏713032623
Create By ifeng<br>
Web Site: https://www.hicairo.com <br>

Telegram: https://t.me/HiaiFeng <br>

# 简介：
本项目用于在 Doprax.com 免费服务上部署 V2ray ，采用的方案为 Nginx + WebSocket + VMess/VLess + TLS。速度与 Replit 相比较慢，但是官方宣传不限流量，服务启动后永不停机。
<br><img src="https://user-images.githubusercontent.com/127408990/224227366-4705c1af-0588-462a-955c-27a97a6da21f.png">
# 注意事项：
<p><b><li>请勿滥用，账号封禁风险自负。</li></b></p>
<p><b><li>部署完成如发现不能上网，请检查域名是否被墙，可使用 Cloudflare CDN 解决。</li></b></p>

# 部署：
<p>1、登录自己的 GitHub 账号后 Fork 该项目。</p>
<p>2、注册 <a href="https://www.doprax.com/signup/">Doprax.com</a> 账号登录后 Import 该项目。</p>
<p>详细使用方案请参考：https://www.hicairo.com/post/55.html</p>

# 使用方法：
<p>1、服务器端配置</p>
<p>请使用 <a href="https://www.v2fly.org/awesome/tools.html">第三方工具</a> 生成一个新的 UUID 。在 Doprax.com 登录后依次点击左侧菜单中的 Main ,窗口右侧的 Edit source code ，选择 Dockerfile 文件，编辑 UUID 及伪装地址信息保存后重启服务。</p>

<img src="https://user-images.githubusercontent.com/127408990/224228204-3a6f1f31-0cef-4624-bee8-fdc1df1204e7.png">
<pre class="notranslate"><code># 用新生成的 UUID 替换 de04add9-5c68-8bab-950c-08cd5320df18
ENV UUID de04add9-5c68-8bab-950c-08cd5320df18
# VMESS_WSPATH / VLESS_WSPATH 两个常量分别定义了 Vmess/VLess 的伪装路径，
# 请分别修改内容中的vmess或vless。注意：伪装路径以 / 符号开始,为避免不必要的麻烦，请不要使用特殊符号.
ENV VMESS_WSPATH /vmess
ENV VLESS_WSPATH /vless
</code></pre>

<p>2、客户端配置</p>
<p>节点客户端配置需要手动进行，下面以 V2rayN 为例。
<p>下图为 VMess 配置示意图，请修改标示内容，其他设置与图片中显示一致。</p>
![image](https://user-images.githubusercontent.com/127408990/224228455-9ae8fe77-f7bf-4e15-8945-3748da27ecea.png)

<img src="https://user-images.githubusercontent.com/127408990/224228455-9ae8fe77-f7bf-4e15-8945-3748da27ecea.png">
<p>下图为 VLess 配置示意图，请修改标示内容，其他设置与图片中显示一致。</p>
![image](https://user-images.githubusercontent.com/127408990/224228483-d0b9fe97-ec65-4c3e-8085-db46cb158440.png)

<img src="https://user-images.githubusercontent.com/127408990/224228483-d0b9fe97-ec65-4c3e-8085-db46cb158440.png">

# 反馈与交流：
<p>在使用过程中，如果遇到问题，请使用Telegram与我联系。（ https://t.me/HiaiFeng ）</p>
<p>大家好，Doprax 非常关注用户使用体验。Hemen 先生及他的团队，为 Doprax 社区创建了 Discord 服务，如果您在使用过程中，遇到 Doprax 平台的相关问题或对平台有一些建议，请使用如下链接与官方联系。

Hello everyone! Doprax pays great attention to user experience. Mr. Hemen and his team have created a Discord service for the Doprax community. If you encounter any problems or have any suggestions related to the Doprax platform during use, please contact the official using the link below.

https://discord.gg/pFnGwTuXjk</p>
