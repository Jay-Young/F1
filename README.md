<p align="center">
  <img src="/media/img/logos/f1.svg"/>
  <br>分享 F1 赛事相关资源，包括比赛录像、纪录片等。
</p>

<p align="center">
  <a href="https://space.bilibili.com/175358"><img src="https://img.shields.io/badge/B%E7%AB%99-Bilibili-blue"></a>
  <a href="https://weibo.com/jayyoung1"><img src="https://img.shields.io/badge/%E6%96%B0%E6%B5%AA-Weibo-red"></a>
</p>

## 2022 赛季

### 电信直播

- 获取直播间信息

```bash
curl "http://h5.nty.tv189.com/api/activity/getcpms?path=/clt4/xtysxkhd/tjysyqd/F1zhibojian/index.json"
```

<details>
<summary>响应结果👈点我查看</summary>

```json
//响应结果示例, 已经 Unicode 解码并格式化
{
	"data": [
		{
			"item": [
				{
					"leftName": "F1美国大奖赛",
					"cover": "https://tp.nty.tv189.com/image/tmpl/2022/10/18/7009357344.jpg",
					"descriptionText": "F1美国大奖赛",
					"endTime": "2022-10-22 04:10:00",
					"clickParam": "1",
					"startTime": "2022-10-22 03:00:00",
					"leftIcon": "https://tp.nty.tv189.com/image/tmpl/2022/09/08/7009346872.png",
					"title": "第一阶段练习赛",
					"clickType": 32,
					"type": 1,
					"liveId": "C8000000000000000001661750675248"
				},
				{
					"leftName": "F1美国大奖赛",
					"cover": "https://tp.nty.tv189.com/image/tmpl/2022/10/18/7009357344.jpg",
					"descriptionText": "F1美国大奖赛",
					"endTime": "2022-10-22 07:40:00",
					"clickParam": "1",
					"startTime": "2022-10-22 06:00:00",
					"leftIcon": "https://tp.nty.tv189.com/image/tmpl/2022/09/08/7009346872.png",
					"title": "第二阶段练习赛",
					"clickType": 32,
					"type": 1,
					"liveId": "C8000000000000000001661750675248"
				}
			],
			"time": "2022-10-22 03:00:00"
		},
		{
			"item": [
				{
					"leftName": "F1美国大奖赛",
					"cover": "https://tp.nty.tv189.com/image/tmpl/2022/10/18/7009357344.jpg",
					"descriptionText": "F1美国大奖赛",
					"endTime": "2022-10-23 04:10:00",
					"clickParam": "1",
					"startTime": "2022-10-23 03:00:00",
					"leftIcon": "https://tp.nty.tv189.com/image/tmpl/2022/09/08/7009346872.png",
					"title": "第三阶段练习赛",
					"clickType": 32,
					"type": 1,
					"liveId": "C8000000000000000001661750675248"
				},
				{
					"leftName": "F1美国大奖赛",
					"cover": "https://tp.nty.tv189.com/image/tmpl/2022/10/18/7009357344.jpg",
					"descriptionText": "F1美国大奖赛",
					"endTime": "2022-10-23 07:10:00",
					"clickParam": "1",
					"startTime": "2022-10-23 06:00:00",
					"leftIcon": "https://tp.nty.tv189.com/image/tmpl/2022/09/08/7009346872.png",
					"title": "排位赛",
					"clickType": 32,
					"type": 1,
					"liveId": "C8000000000000000001661750675248"
				}
			],
			"time": "2022-10-23 03:00:00"
		},
		{
			"item": [
				{
					"leftName": "F1美国大奖赛",
					"cover": "https://tp.nty.tv189.com/image/tmpl/2022/10/18/7009357344.jpg",
					"descriptionText": "F1美国大奖赛",
					"endTime": "2022-10-24 05:20:00",
					"clickParam": "1",
					"startTime": "2022-10-24 03:00:00",
					"leftIcon": "https://tp.nty.tv189.com/image/tmpl/2022/09/08/7009346872.png",
					"title": "正赛",
					"clickType": 32,
					"type": 1,
					"score": " ",
					"liveId": "C8000000000000000001661750980383"
				}
			],
			"time": "2022-10-24 03:00:00"
		}
	],
	"block": 7,
	"type": 1,
	"images": [
		{
			"imageUrl": "https://tp.nty.tv189.com/image/tmpl/2022/06/09/7009328301.png"
		}
	],
	"chGroup": "CN_024"
}
```

</details>

- 直播间: <http://h5.nty.tv189.com/zt/zt2022/sport-live?cid=C8000000000000000001661750675248>

- 1080p 抓流

```bash
curl "http://h5.nty.tv189.com/zt/api/liveroomplay" -d 'liveid=C8000000000000000001661750675248'
```

```json
//响应结果示例
{
	"code": 0,
	"info": "http://liveplay.ctx.tv189.com/live/f1zb-4000k.m3u8?sign=&sid=C8000000000000000001661750675248&msisdn=40000000000&spid=&timestamp=20221020072343&H=115010310149&channelid=01833310&nodeid=&videotype=1&encrypt=******打码******&ua=30&nettype=12&imsi=&guid=******打码******&playseek=1",
	"authresp": []
}
```

- 4K 抓流: 手机上装抓包工具从天翼超高清 app 中抓取, 本周直播信号不需要鉴权

```markdown
http://liveplay.ctx.tv189.com/live/f1zb4k-8m.m3u8?sign=&sid=C8000000000000000001661750980383
```

### 比赛录像

|                                  信号源                                  |                                   微力同步密钥                                    |
| :----------------------------------------------------------------------: | :-------------------------------------------------------------------------------: |
|  ![SkySports_UHD](https://img.shields.io/badge/SkySports-UHD-gold) :gb:  |              B4JQXDOK2IELESYLYUW4EZPACTWR7MOIS3Q5WATVCU3QPNPDYPZDPQ               |
|  ![SkySports_FHD](https://img.shields.io/badge/SkySports-FHD-blue) :gb:  |              B4ALQFLLRUN43435CL6RVCWFMGQ5IMMF7EY2LQH6RLT67QBRFQU54Q               |
|   ![F1TV_PRO_FHD](https://img.shields.io/badge/F1TV_PRO-FHD-blue) :gb:   |              B4LUQA3EMJ6TJBOPCBBEJ52WZZE7OVQMI2DFIKQ4KI625QM472WN4Q               |
| ![天翼超高清_UHD](https://img.shields.io/badge/天翼超高清-UHD-gold) :cn: |              B4Q4GHP2BXL6JOIWGQQAE22VMZSEVQIYP4HFVN4QHGBGGZSRHZF5VQ               |
| ![天翼超高清_UHD](https://img.shields.io/badge/天翼超高清-UHD-gold) :cn: | [在线观看](https://space.bilibili.com/175358/channel/collectiondetail?sid=754362) |
|   ![SkySports_HD](https://img.shields.io/badge/SkySports-HD-blue) :gb:   |            [在线观看](https://racereplay.net/category.php)            |

### 比赛信息

|                    0️⃣                     |                      1️⃣                       |                     2️⃣                      |                         3️⃣                         |                    4️⃣                     |
| :---------------------------------------: | :-------------------------------------------: | :-----------------------------------------: | :------------------------------------------------: | :---------------------------------------: |
|  [巴林大奖赛](/races/2022/R01.README.md)  | [沙特阿拉伯大奖赛](/races/2022/R02.README.md) | [澳大利亚大奖赛](/races/2022/R03.README.md) | [艾米利亚-罗马涅大奖赛](/races/2022/R04.README.md) | [迈阿密大奖赛](/races/2022/R05.README.md) |
| [西班牙大奖赛](/races/2022/R06.README.md) |   [摩纳哥大奖赛](/races/2022/R07.README.md)   | [阿塞拜疆大奖赛](/races/2022/R08.README.md) |     [加拿大大奖赛](/races/2022/R09.README.md)      |  [英国大奖赛](/races/2022/R10.README.md)  |
| [奥地利大奖赛](/races/2022/R11.README.md) |    [法国大奖赛](/races/2022/R12.README.md)    |  [匈牙利大奖赛](/races/2022/R13.README.md)  |     [比利时大奖赛](/races/2022/R14.README.md)      |  [荷兰大奖赛](/races/2022/R15.README.md)  |
| [意大利大奖赛](/races/2022/R16.README.md) |   [新加坡大奖赛](/races/2022/R17.README.md)   |   [日本大奖赛](/races/2022/R18.README.md)   |      [美国大奖赛](/races/2022/R19.README.md)       | [墨西哥城大奖赛](/races/2022/R20.README.md) |
|  [巴西大奖赛](/races/2022/R21.README.md)  |  [阿布扎比大奖赛](/races/2022/R22.README.md)  |
