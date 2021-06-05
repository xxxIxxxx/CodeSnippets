# CodeSnippets

# Xcode 路径

```
~/Library/Developer/Xcode/UserData/CodeSnippets
```

打开路径将文件拖进去
代码块添加后需要重启 Xcode

# Swift

| 快捷键    | 注释                          |
| --------- | ----------------------------- |
| lazytab   | 懒加载属性 tableView          |
| mk        | //MARK: -                     |
| snpmake   | SnapKit make 布局             |
| snpremake | SnapKit remake 布局           |
| initBtn   | UIButton 初始化               |
| initCCell | UICollectionViewCell 初始化   |
| initImgV  | UIImageView 初始化            |
| initLab   | UILable 初始化                |
| initTCell | UITableViewCell 初始化        |
| initView  | UIView 初始化                 |
| ssself    | guard let strongSelf = self   |
| letLab    | UILabel [扩展 1](#扩展-1)     |
| letView   | UIView [扩展 1](#扩展-1)      |
| letBtn    | UIButton [扩展 1](#扩展-1)    |
| letImg    | UIImageView [扩展 1](#扩展-1) |

# OC

| 快捷键     | 注释                          |
| ---------- | ----------------------------- |
| initBtn    | UIButton 初始化               |
| initImgV   | UIImageView 初始化            |
| initLab    | UILable 初始化                |
| initCell   | UITableViewCell 初始化        |
| initView   | UIView 初始化                 |
| initTextF  | UITextField 初始化            |
| pna        | @property (nonatomic, assign) |
| pns        | @property (nonatomic, strong) |
| pnc        | @property (nonatomic, copy)   |
| td         | //TODO:                       |
| mas_make   | Masonry make 布局             |
| mas_remake | Masonry remake 布局           |
| mas_update | Masonry update 布局           |

# 添加功能

## 扩展 1

```
protocol XXXBuilder {}

extension XXXBuilder {
    public func with(configure: (inout Self) -> Void) -> Self {
        var this = self
        configure(&this)
        return this
    }
}

extension NSObject: XXXBuilder {}
```
