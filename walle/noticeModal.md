## NoticeModal

信息提醒，用于弹窗提示信息与通知

> extend 底层模块Modal，



#### parame

| 参数     | 说明       | 是否必填 | 类型   |
| -------- | ---------- | -------- | ------ |
| style    | 弱提醒样式 | 是       | Object |
| parentId | 父级挂载   | 否       | String |



#### Options 

- **showModal({title, content, footer}, onCancel)**

> tyep：Promise

显示通知或信息

| 参数     | 说明                 | 是否必填 | 类型            |
| -------- | -------------------- | -------- | --------------- |
| title    | 通知标题（不填隐藏） | 否       | String/HTMLtext |
| content  | 内容（不填隐藏）     | 否       | String/HTMLtext |
| footer   | 底部                 | 否       | String/HTMLtext |
| onCancel | 关闭弹窗回调         | 否       | Function        |

ex:

```javascript
showModal(
    {
      title: '<h2>通知标题</h2>', 
      content: '弹窗内容', 
      footer: '<b>footer</b>底部'
	},
    () => console.log('弹窗被关闭')
).then(() => console.log('消息弹窗已打开'))
```



- ##### hideModal()

  > tyep：Promise
  
  隐藏结果弹窗
