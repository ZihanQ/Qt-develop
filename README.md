## 扫雷控制台版本(Minesweeper cmd version)

### 已实现功能：

1.左键单击。打开该格子，如果该格子周围3×3区域中有雷，则显示雷的个数；如果地雷个数为0，则显示为0并
打开周围3×3区域中所有未被打开的格子。

2.右键单击标记地雷。如果该位置为未被打开的格子或问题标记的格子，该位置可以被标记为地雷，以"!"显
示。

3.右键单击标记问题。如果该位置为未被打开的格子或地雷标记的格子，该位置可以被标记为问题，以"?"显
示。

4.右键单击取消标记。如果该位置为问题标记或地雷标记的格子，该位置可以被取消标记，恢复为未被打开的格子。

5.双击。当双击位置周围已标记雷数等于该位置数字时操作有效，相当于对该数字周围未标记且未打开的格子均
进行一次左键单击操作。地雷未标记完全时使用双击无效。若数字周围有标错的地雷，则游戏结束。

所有基本功能已全部实现

### 代码优势：

1.基本做到较高的内聚度和较低的耦合度；

2.可维护性较高；

3.鲁棒性较强：手动测试的多种不合法或无效情形都能稳定运行；

### 待完善部分：（1.0.0版本)

1.高内聚，低耦合程度仍可提高；

2.可读性有待提高，注释偏少；

3。测试样例少，尚可能有未知bug存在；
 --2023.4.28

### 第一次更新完善(1.1.0版本)

1.雷数显示可以为负数

2.第二档次雷区大小更新为16*16 (原来第二档次为16*19)

3.修复了取消 “!” 标记后的格子不会被双键递归打开的问题
