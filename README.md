# Nicepage
![Image text](https://github.com/duzhen-cn/Nicepage/blob/master/index.jpg)
### [demo](http://nicezz.com/NicePage/index.html)<br>
### 基于强大的LAYUI框架,通过扩展nicePage.js实现JSON数据格式的自动表格分页和跳转功能,配置简单,上手速度快，兼容IE5+<br>
#### 引入js,css文件夹即可
#### /*只需设置如下内容即可*/
```javascript

	//标准json格式 目前只支持[{a:b,c:d},{a:b,c:d}]此种格式
	var json = [{
		"date": "18日星期四",
		"sunrise": "06:06",
		"high": "高温 16.0℃",
		"low": "低温 9.0℃",
		"sunset": "17:20",
		"aqi": 41.0,
		"fx": "北风",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "19日星期五",
		"sunrise": "06:07",
		"high": "高温 17.0℃",
		"low": "低温 10.0℃",
		"sunset": "17:19",
		"aqi": 66.0,
		"fx": "无持续风向",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "20日星期六",
		"sunrise": "06:08",
		"high": "高温 18.0℃",
		"low": "低温 12.0℃",
		"sunset": "17:18",
		"aqi": 68.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "多云",
		"notice": "阴晴之间，谨防紫外线侵扰"
	}, {
		"date": "21日星期日",
		"sunrise": "06:09",
		"high": "高温 19.0℃",
		"low": "低温 15.0℃",
		"sunset": "17:16",
		"aqi": 57.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阴",
		"notice": "不要被阴云遮挡住好心情"
	}, {
		"date": "22日星期一",
		"sunrise": "06:10",
		"high": "高温 19.0℃",
		"low": "低温 14.0℃",
		"sunset": "17:15",
		"aqi": 49.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阵雨",
		"notice": "阵雨来袭，出门记得带伞"
	}, {
		"date": "18日星期四",
		"sunrise": "06:06",
		"high": "高温 16.0℃",
		"low": "低温 9.0℃",
		"sunset": "17:20",
		"aqi": 41.0,
		"fx": "北风",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "19日星期五",
		"sunrise": "06:07",
		"high": "高温 17.0℃",
		"low": "低温 10.0℃",
		"sunset": "17:19",
		"aqi": 66.0,
		"fx": "无持续风向",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "20日星期六",
		"sunrise": "06:08",
		"high": "高温 18.0℃",
		"low": "低温 12.0℃",
		"sunset": "17:18",
		"aqi": 68.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "多云",
		"notice": "阴晴之间，谨防紫外线侵扰"
	}, {
		"date": "21日星期日",
		"sunrise": "06:09",
		"high": "高温 19.0℃",
		"low": "低温 15.0℃",
		"sunset": "17:16",
		"aqi": 57.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阴",
		"notice": "不要被阴云遮挡住好心情"
	}, {
		"date": "22日星期一",
		"sunrise": "06:10",
		"high": "高温 19.0℃",
		"low": "低温 14.0℃",
		"sunset": "17:15",
		"aqi": 49.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阵雨",
		"notice": "阵雨来袭，出门记得带伞"
	}, {
		"date": "18日星期四",
		"sunrise": "06:06",
		"high": "高温 16.0℃",
		"low": "低温 9.0℃",
		"sunset": "17:20",
		"aqi": 41.0,
		"fx": "北风",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "19日星期五",
		"sunrise": "06:07",
		"high": "高温 17.0℃",
		"low": "低温 10.0℃",
		"sunset": "17:19",
		"aqi": 66.0,
		"fx": "无持续风向",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "20日星期六",
		"sunrise": "06:08",
		"high": "高温 18.0℃",
		"low": "低温 12.0℃",
		"sunset": "17:18",
		"aqi": 68.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "多云",
		"notice": "阴晴之间，谨防紫外线侵扰"
	}, {
		"date": "21日星期日",
		"sunrise": "06:09",
		"high": "高温 19.0℃",
		"low": "低温 15.0℃",
		"sunset": "17:16",
		"aqi": 57.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阴",
		"notice": "不要被阴云遮挡住好心情"
	}, {
		"date": "22日星期一",
		"sunrise": "06:10",
		"high": "高温 19.0℃",
		"low": "低温 14.0℃",
		"sunset": "17:15",
		"aqi": 49.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阵雨",
		"notice": "阵雨来袭，出门记得带伞"
	}, {
		"date": "18日星期四",
		"sunrise": "06:06",
		"high": "高温 16.0℃",
		"low": "低温 9.0℃",
		"sunset": "17:20",
		"aqi": 41.0,
		"fx": "北风",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "19日星期五",
		"sunrise": "06:07",
		"high": "高温 17.0℃",
		"low": "低温 10.0℃",
		"sunset": "17:19",
		"aqi": 66.0,
		"fx": "无持续风向",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "20日星期六",
		"sunrise": "06:08",
		"high": "高温 18.0℃",
		"low": "低温 12.0℃",
		"sunset": "17:18",
		"aqi": 68.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "多云",
		"notice": "阴晴之间，谨防紫外线侵扰"
	}, {
		"date": "21日星期日",
		"sunrise": "06:09",
		"high": "高温 19.0℃",
		"low": "低温 15.0℃",
		"sunset": "17:16",
		"aqi": 57.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阴",
		"notice": "不要被阴云遮挡住好心情"
	}, {
		"date": "22日星期一",
		"sunrise": "06:10",
		"high": "高温 19.0℃",
		"low": "低温 14.0℃",
		"sunset": "17:15",
		"aqi": 49.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阵雨",
		"notice": "阵雨来袭，出门记得带伞"
	}, {
		"date": "18日星期四",
		"sunrise": "06:06",
		"high": "高温 16.0℃",
		"low": "低温 9.0℃",
		"sunset": "17:20",
		"aqi": 41.0,
		"fx": "北风",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "19日星期五",
		"sunrise": "06:07",
		"high": "高温 17.0℃",
		"low": "低温 10.0℃",
		"sunset": "17:19",
		"aqi": 66.0,
		"fx": "无持续风向",
		"fl": "3-4级",
		"type": "晴",
		"notice": "愿你拥有比阳光明媚的心情"
	}, {
		"date": "20日星期六",
		"sunrise": "06:08",
		"high": "高温 18.0℃",
		"low": "低温 12.0℃",
		"sunset": "17:18",
		"aqi": 68.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "多云",
		"notice": "阴晴之间，谨防紫外线侵扰"
	}, {
		"date": "21日星期日",
		"sunrise": "06:09",
		"high": "高温 19.0℃",
		"low": "低温 15.0℃",
		"sunset": "17:16",
		"aqi": 57.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阴",
		"notice": "不要被阴云遮挡住好心情"
	}, {
		"date": "22日星期一",
		"sunrise": "06:10",
		"high": "高温 19.0℃",
		"low": "低温 14.0℃",
		"sunset": "17:15",
		"aqi": 49.0,
		"fx": "南风",
		"fl": "3-4级",
		"type": "阵雨",
		"notice": "阵雨来袭，出门记得带伞"
	}];

	//nameList与widthList的数组长度要一致
	var nameList = ['日期', '日出时刻', '最高温', '最低温', '日落时间', '空气指数', '风向', '风力', '天气', '提示'] //table的列名
	var widthList = [100, 100, 100, 100, 100, 100, 100, 100, 100, 250] //table每列的宽度

	/**
	 * 初始化设置nicepage组件    v1.0
	 *-------------------------------------------------------------
	 * 进行数据组装,与layui交互进行元素渲染
	 *-------------------------------------------------------------
	 * @param    {string}  table     table的div id
	 * @param    {string}  bar     底部分页的div id
	 * @param    {int}  limit     每页默认行数
	 * @param    {string}  color     底部分页的颜色
	 * @param    {array}  layout     底部分页的布局,具体可参考layui api
	 *
	 * @date     2018-10-19
	 * @author   Thomas.dz <hzdz163@163.com>
	 */
	$(function () {
		nicePage.setCfg({
			table: 'table',
			bar: 'pageBar',
			limit: 20,
			color: '#1E9FFF',
			layout: ['count', 'prev', 'page', 'next', 'limit', 'skip']
		});
	});//初始化完成
