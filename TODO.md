# TODO

## 智能纠错

## 弹出模态框滚动条样式bug

## 封装ztree，以及将裁判主文模板内容生成的指令化

## 庭审笔录功能列表（修改，完善）
 1. 页面优化，可编辑区域宽度自适应，部分字段需添加验证条件。
 2. 休庭中撤销功能还未实现。
 3. 庭审笔录在录入过程中实时缓存。（每隔10s本地保存）
 4. 询问阶段需优化。
 5. 页面对应区块对应展示逻辑的修改
 6. 笔录通篇选择性按钮过多，需要优化简洁。
 7. 菜单导航中缺席审理菜单是否显现的判断

## 庭审笔录功能列表（新增）
 1. 庭审笔录可编辑功能（在对应笔录添加按钮，手动点击按钮后，庭审笔录不能再做编辑。默认三天后自动变更为不可编辑状态）
 2. 诉讼参与人对应区块新增，笔录正文所有诉讼参与人展示列表与之对应。
 3. 诉讼参与人中添加负责人的情况，修改对应逻辑。
 4. 法庭询问环节的问题及归纳中斜线部分的选择。
 5. 笔录二级导航间可任意变换顺序，且对应笔录内容区块顺序也要随之移动。
 6. 在法庭调查阶段中的法庭询问、归纳争点、举证质证三处导航设置增减功能。

## 庭审笔录问题总结（保存页面上所有字段，还原模板）
 1. 休庭的实现（用户点击休庭，删除对应内容，还原页面时也要删除对应内容）
 2. 模板的随意删除，修改
 3. 所有可编辑内容区需要使用input或者textArea 导致页面样式混乱
 4. 逻辑，数据结构大量更改，需花费大量时间。

 5. 可修改的区域嵌套后，可能会出现的问题：
 * 1. DOM当中全案要素表对应的标志位可能被删除，导致无法对应到裁判文书。
 * 2. 庭审笔录修改时，无法正确的还原全案要素表中可以编辑的区域，以及对应的事件逻辑。

## 庭审笔录中可修改后可能存在的问题
 1. DOM修改时，可能打乱控件的排列顺序，甚至将控件删除。
 2. 先渲染模板，再渲染。


 ### 庭审信息

 信息核对**业务关联**
 庭审序言->告知事项、是否申请回避、举证期限异议
 法庭调查->归纳争点、举证质证

 庭审序言->庭审组织
 法庭调查->法庭询问

