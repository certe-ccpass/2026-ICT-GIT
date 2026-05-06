# Markdown 教學

animal


## 基礎格式
標題：

---

# 一級標題
```md
# 一級標題
```

## 二級標題
```md
## 二級標題
```

### 三級標題
```md
### 三級標題
```

> 一般來說可以去到 6 級

###### 六級標題
```md
###### 六級標題
```

---

## 強調

*斜體*

```md
*斜體*

或者

_斜體_
```

__粗體__

```md
**粗體**

或者

__粗體__
```


_你可以 **組合** 這些樣式_
```md
_你可以 **組合** 這些樣式_
```

~~刪除線~~
```
~~刪除線~~
```



---

## 列表
### 無序號列表：

- 靈長目
    - 人類
    - 大猩猩
- 爬行目
    - 貓科
    - 犬科
- 食肉目

```md
- 靈長目
    - 人類
    - 大猩猩
- 爬行目
    - 貓科
    - 犬科
- 食肉目
```

### 有序列表
1. 科目一
2. 科目二
3. 科目三

```md
1. 科目一
2. 科目二
3. 科目三
```

---

## 插入圖片
![](https://camo.githubusercontent.com/8aad3083adf41087445ae9952c41207a2f3be4623d0b4154a698754584259c69/687474703a2f2f692e696d6775722e636f6d2f76384956446b612e6a7067)

```md
![](https://camo.githubusercontent.com/8aad3083adf41087445ae9952c41207a2f3be4623d0b4154a698754584259c69/687474703a2f2f692e696d6775722e636f6d2f76384956446b612e6a7067)
```

## 插入鏈接
[link](http://example.com)
```md
[link](http://example.com)
```

[example](http://example.com)
```md
[example](http://example.com)
```

---

## 引用塊
> 有人说，他帮唐僧取到了真经，封了斗战胜佛。从此，留在了灵山。
> 也有人说，那个成佛的根本不是他，真正的他，早就死在了西行路上。
> 还有人说，西游从来都没有发生过。他只不过是说书人杜撰的一只猴子。

```md
> 有人说，他帮唐僧取到了真经，封了斗战胜佛。从此，留在了灵山。
> 也有人说，那个成佛的根本不是他，真正的他，早就死在了西行路上。
> 还有人说，西游从来都没有发生过。他只不过是说书人杜撰的一只猴子。
```

---

## 代碼塊
```python
import pandas as pd
import numpy as np

np.random.seed(42)

years = np.arange(2012,2024)

feature1 = np.random.rand(len(years)) * 100
feature2 = np.random.rand(len(years)) * 50

target = 2 * feature1 + 3 * feature2 + np.random.randn(len(years)) * 10

data = pd.DataFrame(
    {
        'years': years,
        'feature1': feature1,
        'feature2': feature2,
        'target': target
    }
)

print(data)
data.to_csv('full_student_data.csv', index=False)
```

````markdown
```python
import pandas as pd
import numpy as np

np.random.seed(42)

years = np.arange(2012,2024)

feature1 = np.random.rand(len(years)) * 100
feature2 = np.random.rand(len(years)) * 50

target = 2 * feature1 + 3 * feature2 + np.random.randn(len(years)) * 10

data = pd.DataFrame(
    {
        'years': years,
        'feature1': feature1,
        'feature2': feature2,
        'target': target
    }
)

print(data)
data.to_csv('full_student_data.csv', index=False)
```
````

注意，在 \`\`\` 後加上編程語言的名字，例如上面是 `\\\python` 就可以觸發代碼語法高亮顯示


---

## 分割線

```md
---
```

---

## 文章引用

**The quick brown [fox][1], jumped over the lazy [dog][2].**

[1]: https://en.wikipedia.org/wiki/Fox "Wikipedia: Fox"
[2]: https://en.wikipedia.org/wiki/Dog "Wikipedia: Dog"

```md
**The quick brown [fox][1], jumped over the lazy [dog][2].**

[1]: https://en.wikipedia.org/wiki/Fox "Wikipedia: Fox"
[2]: https://en.wikipedia.org/wiki/Dog "Wikipedia: Dog"
```

---

## 非格式化使用符號
使用 `\` 表示後面的符號不用於格式化
\*literally\*

```md
\*literally\*
```

---

## 完成清單（部分支持）
- [ ] 未完成
- [x] 已完成

```
- [ ] 未完成
- [x] 已完成

```

--

## 表格
|名字|年齡|性別|
|-|-|-|
|Bob|20|男|
|Amy|16|女|

## 表格
|名字|
|-|-|-|
|Larry|