---
category: Components
subtitle: 下拉菜单
type: Navigation
title: Dropdown
---

向下弹出的列表。

## 何时使用

当页面上的操作命令过多时，用此组件可以收纳操作元素。点击或移入触点，会出现一个下拉菜单。可在列表中进行选择，并执行相应的命令。

## API

属性如下

| 参数        | 说明             | 类型               | 默认值       |
|-------------|------------------|--------------------|--------------|
| trigger     | 触发下拉的行为   | Array<'click'\|'hover'> | ['hover']        |
| overlay     | 菜单         | [Menu](/components/menu) | -     |
| getPopupContainer | 菜单渲染父节点。默认渲染到 body 上，如果你遇到菜单滚动定位问题，试试修改为滚动的区域，并相对其定位。[示例](http://codepen.io/anon/pen/xVBOVQ?editors=001) | Function(triggerNode) | () => document.body |
| visible     | 菜单是否显示 | boolean   | -           |
| onVisibleChange  | 菜单显示状态改变时调用，参数为 visible | Function(visible) | - |
| placement | 菜单弹出位置：`bottomLeft` `bottomCenter` `bottomRight` `topLeft` `topCenter` `topRight` | String | `bottomLeft` |

菜单可由 `antd.Menu` 取得，可设置 `onSelect` 回调，菜单还包括菜单项 `Menu.Item`，分割线 `Menu.Divider`。

> 注意： Menu.Item 必须设置唯一的 key 属性。

> 如果希望去掉菜单选中的背景效果，可以指定 `<Menu selectedKey={[]}>`.

### Dropdown.Button

| 参数        | 说明             | 类型               | 默认值       |
|-------------|------------------|--------------------|--------------|
| type        | 按钮类型，和 [Button](/components/button/) 一致 | string | 'default' |
| onClick     | 点击左侧按钮的回调，和 [Button](/components/button/) 一致 | Function   | - |
| trigger     | 触发下拉的行为   | Array<'click'\|'hover'> | ['hover']        |
| overlay     | 菜单         | [Menu](/components/menu/) | -     |
| visible     | 菜单是否显示 | boolean   | -           |
| onVisibleChange  | 菜单显示状态改变时调用，参数为 visible | Function | - |
| placement | 菜单弹出位置：`bottomLeft` `bottomCenter` `bottomRight` `topLeft` `topCenter` `topRight` | String | `bottomLeft` |
