
# 更新日志 

## 发布周期
- 修订版本号：每周末会进行日常 bugfix 更新。**如果有紧急的 bugfix，则任何时候都可发布**
- 次版本号：每月发布一个带有新特性的向下兼容的版本。
- 主版本号：含有破坏性更新和新特性，不在发布周期内。

<!-- 更新占位 -->
<log title="1.2.14" date="2021-04-23">
	<log-item title="uni-combox 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-data-picker 组件更新">
		<log-item-text tag-type="fix">
			 非树形数据有 where 属性查询报错的问题
		</log-item-text>
	</log-item>
	<log-item title="uni-fav 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-goods-nav 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-nav-bar 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-notice-bar 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-number-box 组件更新">
		<log-item-text tag-type="fix">
			 uni-number-box 浮点数运算不精确的 bug
		</log-item-text>
		<log-item-text tag-type="fix">
			 uni-number-box change 事件触发不正确的 bug
		</log-item-text>
		<log-item-text tag-type="feat">
			 uni-number-box v-model 双向绑定
		</log-item-text>
	</log-item>
	<log-item title="uni-rate 组件更新">
		<log-item-text tag-type="fix">
			 布局变化后 uni-rate  星星计算不准确的 bug
		</log-item-text>
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入 uni-rate 自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-search-bar 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-steps 组件更新">
		<log-item-text tag-type="perf">
			 添加依赖 uni-icons, 导入后自动下载依赖
		</log-item-text>
	</log-item>
	<log-item title="uni-transition 组件更新">
		<log-item-text tag-type="feat">
			 通过方法自定义动画
		</log-item-text>
		<log-item-text tag-type="feat">
			 custom-class 非 NVUE 平台支持自定义 class 定制样式
		</log-item-text>
		<log-item-text tag-type="perf">
			 动画触发逻辑，使动画更流畅
		</log-item-text>
		<log-item-text tag-type="perf">
			 支持单独的动画类型
		</log-item-text>
		<log-item-text tag-type="perf">
			 文档示例
		</log-item-text>
	</log-item>
</log>


<log title="1.2.13" date="2021-04-14">
	<log-item title="uni-data-checkbox 组件更新">
		<log-item-text tag-type="fix">
			 nvue 下无法选中的问题
		</log-item-text>
	</log-item>
	<log-item title="uni-data-picker 组件更新">
		<log-item-text tag-type="feat">
			 支持云端非树形表结构数据
		</log-item-text>
		<log-item-text tag-type="fix">
			 根节点 parent_field 字段等于null时选择界面错乱问题
		</log-item-text>
	</log-item>
	<log-item title="uni-file-picker 组件更新">
		<log-item-text tag-type="fix">
			 选择的文件非 file-extname 字段指定的扩展名报错的Bug
		</log-item-text>
		<log-item-text tag-type="perf">
			 更新组件示例
		</log-item-text>
		<log-item-text tag-type="perf">
			 file-extname 字段支持字符串写法，多个扩展名需要用逗号分隔
		</log-item-text>
	</log-item>
	<log-item title="uni-pagination 组件更新">
		<log-item-text tag-type="feat">
			 PC 和 移动端适配不同的 ui
		</log-item-text>
	</log-item>
	<log-item title="uni-date-picker 组件更新">
		<log-item-text tag-type="perf">
			 发布第一版
		</log-item-text>
	</log-item>
	<log-item title="uni-data-picker 组件更新">
		<log-item-text tag-type="fix">
			 本地数据概率无法回显时问题
		</log-item-text>
	</log-item>
	<log-item title="uni-nav-bar 组件更新">
		<log-item-text tag-type="perf">
			 uni-ui 修复 uni-nav-bar 当 fixed 属性为 true 时铺不满屏幕的 bug
		</log-item-text>
	</log-item>
	<log-item title="uni-rate 组件更新">
		<log-item-text tag-type="fix">
			 uni-rate 属性 margin 值为 string 组件失效的 bug
		</log-item-text>
	</log-item>
	<log-item title="uni-search-bar 组件更新">
		<log-item-text tag-type="perf">
			 uni-ui 新增 uni-search-bar 的 focus 事件
		</log-item-text>
	</log-item>
	<log-item title="uni-table 组件更新">
		<log-item-text tag-type="feat">
			 sortable 属性，是否开启单列排序
		</log-item-text>
		<log-item-text tag-type="perf">
			 表格多选逻辑
		</log-item-text>
	</log-item>
</log>

<log title="组件工程调整" date="2020-02-05">
	<log-item-text tag-type="docs" only>
		支持uni_modules
	</log-item-text>
</log>

<log title="1.2.11" date="2021-1-19">
	<log-item-text tag-type="feat" only>
		<highlight text="uni-row" /> 栅格系统
	</log-item-text>
	<log-item-text tag-type="feat" only>
		<highlight text="uni-data-picker" /> 数据驱动的picker选择器
	</log-item-text>
	<log-item-text tag-type="feat" only>
		<highlight text="uni-file-picker" /> 文件选择上传
	</log-item-text>
	<log-item title="uni-forms 组件更新">
		<log-item-text tag-type="fix">
			偶发性获取表单值错误的Bug
		</log-item-text>
		<log-item-text tag-type="fix">
			校验 uni-data-picker value 为 0 时，返回值错误的Bug
		</log-item-text>
		<log-item-text tag-type="fix">
			uni-forms-item 组件隐藏时依然触发校验的bug
		</log-item-text>
		<log-item-text tag-type="perf">
			实时校验
		</log-item-text>
	</log-item>
	<log-item title="uni-fab 组件更新">
		<log-item-text tag-type="perf">
			背景色调整
		</log-item-text>
	</log-item>
	<log-item title="组件 NVUE 化">
		<log-item-text tag-type="perf">
			<highlight text="uni-forms" /> 表单
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-easyinput" /> 输入框
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-group" /> 分组
		</log-item-text>
	</log-item>
	<log-item title="组件适配 PC">
		<log-item-text tag-type="perf">
			<highlight text="uni-fab" /> 悬浮按钮
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-swiper-dot" /> 轮播图指示点
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-rate" /> 评分
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-notice-bar" /> 通告栏
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-indexed-list" /> 索引列表
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-combox" /> 组合框
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-transition" /> 动画
		</log-item-text>
		<log-item-text tag-type="perf">
			<highlight text="uni-swipe-action" /> 滑动操作
		</log-item-text>
	</log-item>
</log>

<log title="官网更新" date="2020-12-19">
	<log-item-text tag-type="docs" only>
		整理组件文档
	</log-item-text>
	<log-item-text tag-type="docs" only>
		右侧编辑器跟随滚动，适应小屏设备
	</log-item-text>
	<log-item-text tag-type="docs" only>
		优化 md 的代码块显示样式
	</log-item-text>
</log>

<log title="1.2.10" date="2020-12-18">
	<log-item title="uni-forms 组件更新">
		<log-item-text tag-type="fix">
			不设置 label 属性的时候 errorMessage 位置错误的问题
		</log-item-text>
	</log-item>
	<log-item title="uni-list 组件更新">
		<log-item-text tag-type="fix">
			uni-list-chat 扩展组件角标显示不正常的问题
		</log-item-text>
	</log-item>
	<log-item title="uni-easyinput 组件更新">
		<log-item-text tag-type="feat">
			styles 属性，可以自定义部分样式
		</log-item-text>
		<log-item-text tag-type="feat">
			图标点击事件
		</log-item-text>
		<log-item-text tag-type="fix">
			校验返回值与实际返回值不一致的问题
		</log-item-text>
	</log-item>
	<log-item title="data-checkbox 组件更新">
		<log-item-text tag-type="fix">
			异步获取数据渲染失败的Bug
		</log-item-text>
		<log-item-text tag-type="fix">
			支付宝小程序端报错且显示不正常的Bug
		</log-item-text>
		<log-item-text tag-type="fix">
			z-index 错误的Bug
		</log-item-text>
		<log-item-text tag-type="perf">
			兼容属性 disabled
		</log-item-text>
	</log-item>
	<log-item title="uni-indexed-list 组件更新">
		<log-item-text tag-type="fix">
			easyCom 模式下，找不到子组件的问题
		</log-item-text>
	</log-item>
	
</log>

<log title="1.2.9" date="2020-12-04">
	<log-item-text tag-type="feat" only>
		<highlight text="uni-easyinput" /> 增强输入框
	</log-item-text>
	<log-item-text tag-type="feat" only>
		<highlight text="uni-data-checkbox" /> 数据驱动的单选复选框
	</log-item-text>
	<log-item-text tag-type="feat" only>
		<highlight text="uni-dateformat" /> 日期格式化
	</log-item-text>
	<log-item title="uni-list 组件更新">
		<log-item-text tag-type="fix">
			uni-list-chat 扩展组件角标显示不正常的问题
		</log-item-text>
	</log-item>
</log>

<log title="1.2.8" date="2020-10-23">
	<log-item-text tag-type="feat" only>
		<highlight text="uni-forms" /> 表单组件
	</log-item-text>
	<!-- <log-item-text tag-type="feat" only>
		<highlight text="uni-field" /> 输入框组件
	</log-item-text> -->
	<log-item-text tag-type="feat" only>
		<highlight text="uni-group" /> 分组组件
	</log-item-text>
	<log-item-text tag-type="feat" only>
		<highlight text="uni-table" /> 表格组件
	</log-item-text>
</log>

<log title="1.2.5" date="2020-08-14">
	<log-item title="uni-list 组件更新">
		<log-item-text tag-type="feat">
			更新更多模板示例
		</log-item-text>
		<log-item-text tag-type="feat">
			direction 属性，可以改变列表的排版方向
		</log-item-text>
		<log-item-text tag-type="fix">
			uni-list-chat 组件添加 to 属性，@click 事件不触发的Bug
		</log-item-text>
		<log-item-text tag-type="perf">
			to 属性可单独设置
		</log-item-text>
	</log-item>
	<log-item title="uni-fab 组件更新">
		<log-item-text tag-type="perf">
			按钮缺省时，可直接点击大按钮
		</log-item-text>
	</log-item>
	<log-item title="uni-rate 组件更新">
		<log-item-text tag-type="fix">
			超出设置星星的长度，还可以继续选择的Bug
		</log-item-text>
	</log-item>
</log>


<log title="1.2.4" date="2020-08-13">
	<log-item-text tag-type="perf" only>
		<highlight text="uni-ui" /> 项目结构优化
	</log-item-text>
	<log-item-text tag-type="docs" only>
		 添加日志显示
	</log-item-text>
	<log-item title="uni-list 组件更新">
		<log-item-text tag-type="feat">
			clickable 属性，是否开启点击反馈
		</log-item-text>
		<log-item-text tag-type="feat">
			link 属性，显示右侧箭头并开启点击反馈
		</log-item-text>
		<log-item-text tag-type="feat">
			to 属性，直接跳转到指定页面
		</log-item-text>
		<log-item-text tag-type="feat">
			  border 属性，是否显示列表分割线
		</log-item-text>
	</log-item>
	<log-item title="uni-rate 组件更新">
		<log-item-text tag-type="feat">
			  disabled 属性，可设置组件禁用状态（之前版本的不可点击状态）
		</log-item-text>
		<log-item-text tag-type="feat">
			  disabledColor 属性，可设置禁用颜色
		</log-item-text>
		<log-item-text tag-type="feat">
			  readonly 属性，可设置组件只读属性
		</log-item-text>
		<log-item-text tag-type="feat">
			  allowHalf 属性，可设置组件是否开启半星选择
		</log-item-text>
		<log-item-text tag-type="feat">
			  touchable 属性，可设置组件是否支持滑动手势
		</log-item-text>
		<log-item-text tag-type="fix">
			  动态传值不更新的问题
		</log-item-text>
		<log-item-text tag-type="perf">
			  value 属性可使用 v-model 双向绑定数据
		</log-item-text>
	</log-item>
	<log-item title="uni-popup 组件更新">
		<log-item-text tag-type="perf">
			  扩展组件支持 easycom
		</log-item-text>
	</log-item>
	<log-item title="uni-swipe-action 组件更新">
		<log-item-text tag-type="feat">
			  新增左侧滑动方式
		</log-item-text>
		<log-item-text tag-type="feat">
			  新增插槽使用方式
		</log-item-text>
		<log-item-text tag-type="feat">
			  threshold 属性，可以控制滑动缺省值
		</log-item-text>
		<log-item-text tag-type="fix">
			 滚动页面时触发组件滑动的Bug
		</log-item-text>
		<log-item-text tag-type="perf">
			  优化长列表滚动性能
		</log-item-text>
	</log-item>
</log>

<log title="0.0.1" date="2020-08-12">
	<log-item-text tag-type="docs" only>
		  uni-ui 文档初始化更新
	</log-item-text>
</log>

