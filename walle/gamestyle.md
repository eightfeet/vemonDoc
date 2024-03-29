# 游戏皮肤GameTheme

配置一个完整的抽奖活动皮肤包含**游戏皮肤**与**[模块皮肤](./modulesstyle.md)**两块，其结构如下：

```javascript
Theme = {
    // GameTheme 游戏皮肤
  "GameTheme": {},
	// 模块皮肤
  "FailedModalTheme": {},
  "SuccessModalTheme": {},
  "AddressModalTheme": {},
  "MessageTheme": {},
  "LoadingTheme": {}

}
```

> 1. 所有概率抽奖游戏的模块皮肤结构是一致的，但游戏形式不一样导致游戏皮肤结构会有所不同
> 2. 通常说GameTheme包含的所有属性值是一个CSSStyle对象,css属性名支持中横线的写法，但建议使用javascript定义的css驼峰写法，游戏模块中通过解析器将它们转换为html行内样式进行自定义皮肤渲染
> 3. GameTheme的modify（修饰器）他的属性值 是一个数组，每个数组元素对应会创建一个 基于游戏绝对定位div层，用于修饰游戏模块



### 游戏皮肤结构

​	[大转盘抽奖](#a) 

​	[九宫格抽奖](#b) 

​	[翻牌抽奖](#c) 

​	[红包抽奖](#d) 

​	[掷色子抽奖](#e)

​	[老虎机抽奖](#f)



- ##### <span id="a">大转盘抽奖</span>

  ```javascript
  GameTheme = {
      // 外框
  	"wrap": {"zIndex": 10 }, 
      // 游戏图片
      "gameImg": {},
      // 奖品别名
      "prizeAlias": {},
      // 指针
      "needle": {},
      // 抽奖按钮
      "lotteryButton": {},
      // 转盘
      "wheel": {},
      // 转盘分割线
      "divide": {},
      // 修饰层
      "modify": [{"top": "-2.56em"},{...}]
  }
  ```

  

- ##### <span id="b">九宫格抽奖</span>

  ```javascript
  GameTheme = {
  	// 外框
  	"wrap": {},
      // 游戏图片
      "gameImg": {},
      // 奖品图片
      "prize": {},
      // 激活或者被选中
      "activated": {},
      // 奖品别名
      "prizeAlias": {},
      // 指针
      "needle": {},
      // 抽奖按钮
      "lotteryButton": {},
      // 修饰层
      "modify": []
  }
  ```

  

- ##### <span id="c">翻牌抽奖</span>

  ```javascript
  GameTheme = {
      // 外框
      "wrap": {},
      // 卡牌外框
      "cardWrap": {},
      // 卡牌内容
      "cardInside": {},
      // 卡牌封面
      "cardCover": {},
      // 卡牌内容被选中
      "cardSelected": {},
      // 奖品图片
      "prizeImage": {},
      // 奖品名称
  	"prizeTitle": {},
      // 修饰层
  	"modify": [{}]
  }
  ```



- ##### <span id="d">红包抽奖</span>

  ```javascript
  GameTheme = {
  	// 外框
      "wrap": {},
      // 封面
      "cover": {},
      // 封底
      "backCover": {},
      // 封面文字
      "coverTexts": {},
      // 封面标题
      "coverTitle": {},
      // 封面次标题
      "coverSubTitle": {},
      // 游戏结果
      "gameResult": {},
      // 获奖名字
      "gameResultPrizename": {},
      // 获奖信息
      "gameResultAwardMsg": {},
      // 奖品备注
      "gameResultMemo": {},
      // 确定操作按钮
      "ensureBtn": {},
      // 开始按钮
      "startButton": {},
      // 显示活动信息按钮
      "showGameInfoButton": {},
      // 活动信息布局
      "gameInfoLayout": {},
      // 活动信息外框
      "gameInfoWrap": {},
      // 活动信息奖品单项
      "gameInfoPrizeItem": {},
      // 活动信息单项图片
      "gameInfoPrizeImg": {},
      // 活动信息奖品名称
      "gameInfoPrizeName": {},
      // 修饰层
      "modify": []
  }
  ```

  

- ##### <span id="e">掷色子抽奖</span>

  ```javascript
  GameTheme = {
  	"wrap": {},
      // 显示活动信息按钮
      "showGameInfoButton": {},
      // 活动信息布局
      "gameInfoLayout": {},
      // 活动信息外框
      "gameInfoWrap": {},
      // 活动信息奖品单项
      "gameInfoPrizeItem": {},
      // 活动信息单项图片
      "gameInfoPrizeImg": {},
      // 活动信息奖品名称
      "gameInfoPrizeName": {},
      // 对照标签
      "gameInfoPrizeTag": {},
      // 色子
      "dice": {},
      // 色子的一个面
      "side": {},
      // 色子上的点
      "dot": {},
      // 修饰层
      "modify": []
  }
  ```

  

- ##### <span id="f">老虎机</span>

  ```javascript
  GameTheme = {
      
      // 外框
      "wrap": {},
      // 开始按钮
      "startButton": {},
      // 显示活动信息按钮
      "showGameInfoButton": {},
      // 活动信息布局
      "gameInfoLayout": {},
      // 活动信息外框
      "gameInfoWrap": {},
      // 活动信息奖品单项
      "gameInfoPrizeItem": {},
      // 活动信息单项图片
      "gameInfoPrizeImg": {},
      // 活动信息奖品名称
      "gameInfoPrizeName": {},
      // 游戏单项
      "gameItem": {},
      // 游戏奖项标题
      "gamePrizeName": {},
      // 游戏奖项图片
      "gamePrizeImg": {},
      // 游戏
      "game": {},
      // 修饰层
      "modify": []
  }
  ```

  
