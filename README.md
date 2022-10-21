<p align="center">
  <img src="/media/img/logos/f1.svg"/>
  <br>分享 F1 赛事相关资源，包括比赛录像、纪录片等。
</p>

<p align="center">
  <a href="https://space.bilibili.com/175358"><img src="https://img.shields.io/badge/B%E7%AB%99-Bilibili-blue"></a>
  <a href="https://weibo.com/jayyoung1"><img src="https://img.shields.io/badge/%E6%96%B0%E6%B5%AA-Weibo-red"></a>
</p>

> 说明: 🟢 代表该站比赛页面创建完成 🔴 代表该站比赛页面还未创建 🟡 代表该站比赛页面施工中，一般为正在进行的比赛实时更新中

## 2022 赛季

- 获取直播间 cid

```bash
curl "http://h5.nty.tv189.com/api/portal/act/yylist?startTime=20221022030000&endTime=20221024050000" -H 'Cookie: c_t_id=******打码******;'
#c_t_id 值即登陆后的 token, 浏览器有效期为一个月, 不加登录 token 返回错误
#startTime 和 endTime 随意只要符合格式要求即可, 返回的似乎必然是当前站的直播信息
```

```json
//预期返回结果示例
{
	"code": 0,
	"data": [
		{
			"appointId": "C8000000000000000001661750675248", //直播间 cid
			"startTime": "2022-10-22 03:00:00",
			"endTime": "2022-10-22 04:10:00"
		}
	],
	"total": 1
}
```

- 美国站电信直播: <http://h5.nty.tv189.com/zt/zt2022/sport-live?cid=C8000000000000000001661750675248>

- 1080p 抓流

```bash
curl "http://h5.nty.tv189.com/zt/api/liveroomplay" -d 'liveid=C8000000000000000001661750675248'
```

```json
//预期返回结果示例
{
  "code": 0,
  "info": "http:\/\/liveplay.ctx.tv189.com\/live\/f1zb-4000k.m3u8?sign=&sid=C8000000000000000001661750675248&msisdn=40000000000&spid=&timestamp=20221020072343&H=115010310149&channelid=01833310&nodeid=&videotype=1&encrypt=******打码******&ua=30&nettype=12&imsi=&guid=******打码******&playseek=1",
  "authresp": []
}
```

- 4K 抓流: 手机上装抓包工具从天翼超高清app中抓取

### 比赛录像

|                                  信号源                                  |                                   微力同步密钥                                    |
| :----------------------------------------------------------------------: | :-------------------------------------------------------------------------------: |
|  ![SkySports_UHD](https://img.shields.io/badge/SkySports-UHD-gold) :gb:  |              B4JQXDOK2IELESYLYUW4EZPACTWR7MOIS3Q5WATVCU3QPNPDYPZDPQ               |
|  ![SkySports_FHD](https://img.shields.io/badge/SkySports-FHD-blue) :gb:  |              B4ALQFLLRUN43435CL6RVCWFMGQ5IMMF7EY2LQH6RLT67QBRFQU54Q               |
|   ![F1TV_PRO_FHD](https://img.shields.io/badge/F1TV_PRO-FHD-blue) :gb:   |              B4LUQA3EMJ6TJBOPCBBEJ52WZZE7OVQMI2DFIKQ4KI625QM472WN4Q               |
| ![天翼超高清_UHD](https://img.shields.io/badge/天翼超高清-UHD-gold) :cn: |              B4Q4GHP2BXL6JOIWGQQAE22VMZSEVQIYP4HFVN4QHGBGGZSRHZF5VQ               |
| ![天翼超高清_UHD](https://img.shields.io/badge/天翼超高清-UHD-gold) :cn: | [在线观看](https://space.bilibili.com/175358/channel/collectiondetail?sid=754362) |

### 比赛信息

| 0️⃣                                                     | 1️⃣                                                                    | 2️⃣                                                          | 3️⃣                                                         | 4️⃣                                                       |
| ------------------------------------------------------ | --------------------------------------------------------------------- | ----------------------------------------------------------- | ---------------------------------------------------------- | -------------------------------------------------------- |
| 🟢 :bahrain: [巴林大奖赛](/races/2022/R01.README.md)   | 🟢 :saudi_arabia: [沙特阿拉伯大奖赛](/races/2022/R02.README.md)       | 🟢 :australia: [澳大利亚大奖赛](/races/2022/R03.README.md)  | 🟢 :it: [艾米利亚-罗马涅大奖赛](/races/2022/R04.README.md) | 🔴 :us: [迈阿密大奖赛](/races/2022/R05.README.md)        |
| 🔴 :es: [西班牙大奖赛](/races/2022/R06.README.md)      | 🔴 :monaco: [摩纳哥大奖赛](/races/2022/R07.README.md)                 | 🔴 :azerbaijan: [阿塞拜疆大奖赛](/races/2022/R08.README.md) | 🔴 :canada: [加拿大大奖赛](/races/2022/R09.README.md)      | 🔴 :gb: [英国大奖赛](/races/2022/R10.README.md)          |
| 🔴 :austria: [奥地利大奖赛](/races/2022/R11.README.md) | 🔴 :fr: [法国大奖赛](/races/2022/R12.README.md)                       | 🔴 :hungary: [匈牙利大奖赛](/races/2022/R13.README.md)      | 🔴 :belgium: [比利时大奖赛](/races/2022/R14.README.md)     | 🔴 :netherlands: [荷兰大奖赛](/races/2022/R15.README.md) |
| 🟢 :it: [意大利大奖赛](/races/2022/R16.README.md)      | 🟢 :singapore: [新加坡大奖赛](/races/2022/R17.README.md)              | 🟢 :jp: [日本大奖赛](/races/2022/R18.README.md)             | 🟡 :us: [美国大奖赛](/races/2022/R19.README.md)            | 🔴 :mexico: [墨西哥大奖赛](/races/2022/R20.README.md)    |
| 🔴 :brazil: [巴西大奖赛](/races/2022/R21.README.md)    | 🔴 :united_arab_emirates: [阿布扎比大奖赛](/races/2022/R22.README.md) |
