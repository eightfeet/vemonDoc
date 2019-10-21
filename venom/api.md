# @byhealth/lottery

### Install

```
npm install @byhealth/lottery -S
```

#### 包目录结构

```
node_modules
	└─@byhealth/lottery
		└─lib
			├─ roulette // 大转盘抽奖
			├─ boxroulette // 九宫格抽奖
			├─ flipcard // 翻牌抽奖
			├─ redenvelope // 红包抽奖
			├─ dice // 掷色子抽奖
			└─ slotmachine // 老虎机抽奖
```

### options

| 名称         | 类型                | 说明                                     |
| ------------ | ------------------- | ---------------------------------------- |
| Game         | Classes Constructor | 游戏核心模块，定义游戏形式和抽奖主要流程 |
| NoticeModal  | Classes Constructor | 消息弹窗模块                             |
| Loading      | Classes Constructor | Loading模块                              |
| Message      | Classes Constructor | 弱提示模块                               |
| Modal        | Classes Constructor | 底层弹窗模块                             |
| AddressModal | Classes Constructor | 中奖地址收集弹窗模块                     |
| inlineStyle  | Function            | 行内样式格式工具                         |
| validate     | Function            | 表单验证工具                             |



