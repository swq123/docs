# MoonSwap App 小程序体验

## 简介
在区块链行业内，市面上很多产品出现访问被墙，应用加载慢等现象，用户体验极差。
DAppStore 提供的小程序加载体验，已集成到App中，是一种Web加速方式，开发者按要求接入后，即可获得小程序能力，秒开DApp。

## 接入规范

- 准备资源包

将源代码或者是加密后的代码，build一份，压缩，解压后的文件夹名称为source，source里面为源代码，跟source平级的您可以放一些其他的需要网络请求但是更新不是很频繁的文件，参考下图

![image](/assets/source_demo.png)

- 配置信息

| 名称 | 描述 | 示例 |
| --- | --- | --- |
| baseUrl | 网站的Url  | https://app.uniswap.org|
| 入口路径 | 默认打开的Path | /#/add/0xdAC17F958D2ee523a2206206994597C13D831ec7/0x6B175474E89094C44Da98b954EedeAC495271d0F |
| web入口文件 | 默认为index.html | - |
|版本号 | - | 1.0.1 |

- 自定义映射Mapping

当一些静态资源被档在墙外，可通过自定义映射来满足正常访问。

`demo`

|网络请求链接 | 资源路径 |
| --- | --- |
| https://app.uniswap.org/locales/zh.json  | /otherfiles/zh.json|
| https://cloudflare-ipfs.com/ipns/tokens.uniswap.org | http://jdgjfile-1251031594.file.myqcloud.com/cd2a23fd5adb0b2f0195128d1c37dc4f.json |

- 自定义小程序Menu

支持开发者为小程序添加菜单功能，需要提供:

-- icon图标
-- 按钮名称
-- 跳转目标链接

效果如图:

!(image)[/assets/custom_menu.jpeg]


## 资源包上传

开发者如果有需求，可联系 sky:(微信：BDMoonSwap)

后续会开发方便开发者自主上传的开放平台。
