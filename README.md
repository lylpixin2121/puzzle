# puzzle

puzzle.js是一个基于移动端的拼图游戏插件。

### puzzle.js功能特点：

- **自定义模块高度** ：没啥好说的 (～﹃～)~zZ
- **自定义控制行列数量** ：比如三行四列 五行三列 等等
- **自定义拼图背景** ：可以扩展为多张图的自定义添加或者是随机图之类的 
- **允许自定义板块序列** ：默认情况下 是随机排列的
- **必要的回调时间** ：成功回调

> **目前并没有将拼图游戏中的倒计时环节加入其中**

---

### update 列表

#### (2016-06-28)

- 【修复】修复 多手指滑动下暴力测试引起的定位 bug
- 【优化】优化算法逻辑
- 【优化】动态创建了拖动元素
- 【优化】动态创建了遮罩层元素
- 【新增】新增了自定义随机序列的排序功能
- 【新增】新增了自定义背景图功能

#### (2016-06-30)

- 【修复】修复 自定义背景图中的一些小 bug

#### (2016-07-04)

- 【新增】自动添加data-num标示
- 【新增】允许自定义宽高列数，并自动计算对比序列
- 【优化】添加了一些人性化的Error提示。 

#### (2016-07-13)
- 【优化】动态添加background-position

#### 快速使用


#### js调用
``` 
	puzzle = new Puzzle({
	    itemWidth : 97,
	    itemHeight : 117,
	    rows : 3,
	    column : 3,
	    bgImg : "2.jpg",
	    success : function(){
	        alert("游戏成功！");
	    }
	});
```

[【Demo】](http://192.168.50.198/2016pclady/201606/choice_pintu/puzzle/puzzle.html)


| 参数|说明| 默认值|
| :-------- | :--------| :--: |
| container| 拼图区域最外围的包裹容器，选填 类型 String| “#puzzleBox”  |
| item|    容器内的拼图板块，选填 类型 String| 	“.item”  |
| itemWidth|    	拼图板块的宽度 类型 Number| 	300 |
| itemHeight|    拼图板块的高度 类型 Number| 	300  |
| rows|    拼图区域的行数 类型 Number| 	3  |
| column|    拼图区域的列数 类型 Number| 	3  |
| bgImg|    拼图板块的背景图，必填项 类型 String| 	无  |
| isRandom|    是否随机排列拼图板块 类型 Boolean | 	true  |
| sortArr|    自定义板块顺序序列，此参数仅当isRandom为false时有效，类型 Array | 	false  |
| success|    	拼图成功的回调 类型 Function| 	无  |












         