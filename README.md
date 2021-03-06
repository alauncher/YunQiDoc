### 云启管控

> 版本信息.

<center>
<table>
  <tr>
    <th>日期</th>
    <th>修订版本</th>
    <th>修订内容</th>
    <th>作者</th>
  </tr>
  <tr>
    <td>2019.1.10</td>
    <td>Draft</td>
    <td>Create</td>
    <td>xxx</td>
  </tr>
  <tr>
    <td>2019.1.17</td>
    <td>Draft</td>
    <td>Update</td>
    <td>xxx</td>
  </tr>
  <tr>
    <td>2019.3.19</td>
    <td>Draft</td>
    <td>Update</td>
    <td>xxx</td>
  </tr>
</table>
</center>
</br>


##### 一、 系统定制

序号 | 需求 | 备注
:-:|---|---
1 | 禁用系统 "双清" 功能 | 包括同时按“电源” + “音量+” 能恢复出厂设置等
2 | 禁用安全模式功能 |
3 | 禁用工厂测试模式 |
4 | 禁用飞行模式; |
5 | 禁止长按Home、多任务键的功能 |
6 | 禁止系统 "状态栏" 下拉 |
7 | 禁用Android通知功能，且状态栏不显示通知图标 |
8 | 去掉所有开机向导 |
9 | 默认允许安装未知来源apk |
10 | 默认解锁方式为无 |
11 | 默认休眠状态下保持WLAN连接默认为始终 |
12 | 默认打开自动同步时间和日期且使用24小时制 |
</br>

</br>

##### 二、接口提供

###### 1. 设备控制

序号 | 需求 | 备注
:-:|---|---
1 | 禁用/启用 使用摄像头; | 禁用后用户无法通过任何方式调用摄像头；
2 | 禁用/启用 蓝牙功能; |
3 | 禁用/启用 TF卡; |
4 | 禁用/启用 GPS功能; |
5 | 禁用/启用 短信功能; |
6 | 禁用/启用 通话功能; |
7 | 禁用/启用 USB仅充电; | 开启后，平板为仅充电模式，数据线连接平板后无法查看其SD卡内容，</br>无法ADB调试；此时连线不弹出USB连接对话框。</br>关闭后，可查看SD卡内容，可ADB调试。
8 | 禁用/启用 NFC功能; |
</br>

</br>

###### 2. 应用安装白名单

序号 | 需求 | 备注
:-:|---|---
1 | 设置一个包名集合作为应用安装白名单; | 在白名单集合内的应用包名，可以安装，否则不可安装；
2 | 添加包名到应用白名单; |
3 | 删除应用白名单里指定的包名; |
4 | 获取当前可安装应用白名单; | 获取可以安装应用白名单的集合；

</br>

</br>

###### 3. 静默安装/卸载

序号 | 需求 | 备注
:-:|---|---
1 | 静默安装应用; | 
2 | 静默卸载应用; | 

</br>

</br>

###### 4. 全局网络白名单

序号 | 需求 | 备注
:-:|---|---
1 | 设置网络白名单集合; | 设置网络白名单集合后，设备中除了白名单集合内的域名/IP之外，皆不可上网 |
2 | 获取全局的网络白名单; |
3 | 清空网络白名单集合; | 清空后，设备恢复正常上网;

</br>

</br>

###### 5. 应用网络白名单

序号 | 需求 | 备注
:-:|---|---
1 | 以包名集合作为参数设置应用网络白名单 | 设置后的应用可上网，且不受全局网络白名单的影响 |
2 | 获取应用网络白名单; |
3 | 清空应用网络白名单; | 
</br>

</br>

###### 6. 主界面（Launcher）

序号 | 需求 | 备注
:-:|---|---
1 | 设置默认Launcher; |  |


</br>

</br>

###### 7. 导航栏（StatusBar）

序号 | 需求 | 备注
:-:|---|---
1 | 隐藏/显示 Recent按键; |  |
2 | 隐藏/显示 Home按键; |  |
3 | 隐藏/显示 Back按键; |  |


</br>

</br>

###### 8. 其他

序号 | 需求 | 备注
:-:|---|---
1 | 截屏; | 调用接口获取截屏并返回图片; |
2 | 熄屏幕/亮屏; | 调用接口控制设备屏幕亮灭; |
3 | 关机; | 提供接口，调用后设备关机; |
4 | 重启; | 提供接口，调用后设备重启; |
5 | 恢复出厂设置; | 提供接口，调用后设备恢复出厂设置; |