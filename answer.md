# 第1次隨堂-隨堂-QZ1
>
>學號：112111205
><br />
>姓名：鄭宇辰
><br />
>作業撰寫時間：40 (mins，包含程式撰寫時間)
><br />
>最後撰寫文件日期：2024/9/30
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x] 說明內容
- [x] 個人認為完成作業須具備觀念

## 說明程式與內容

開始寫說明，該說明需說明想法，
並於之後再對上述想法的每一部分將程式進一步進行展現，
若需引用程式區則使用下面方法，
若為.cs檔內程式除了於敘述中需註明檔案名稱外，
還需使用語法` ```語言種類 程式碼 ``` `，其中語言種類若是要用python則使用py，java則使用java，C/C++則使用cpp，
下段程式碼為語言種類選擇csharp使用後結果：

```csharp
public void mt_getResult(){
    ...
}
```

若要於內文中標示部分網頁檔，則使用以下標籤` ```html 程式碼 ``` `，
下段程式碼則為使用後結果：

```html
<%@ Page Language="C#" AutoEventWireup="true" ...>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
<meta http-equiv="Content-Type" ...>
    <title></title>
</head>
<body>
    <form id="form1" runat="server">
        <div>
        </div>
    </form>
</body>
</html>
```

更多markdown方法可參閱[https://ithelp.ithome.com.tw/articles/10203758](https://ithelp.ithome.com.tw/articles/10203758)

請在撰寫"說明程式與內容"該塊內容，請把原該塊內上述敘述刪除，該塊上述內容只是用來指引該怎麼撰寫內容。

1. 請參閱投影片Topic0_1的第37頁，並於專案下開啟一個1.py的檔案，將該頁程式鍵入後，請再依照程式內的person1實例，再生成一個person2，並觀察和person1的差異
```py
class Person:
    name: str
    age: int

    def __init__(self, name: str, age: int):
        self.name = name
        self.age = age

    def greet(self) -> str:
        return f"Hello, my name is {self.name} and I am {self.age} years old."

    def haveBirthday(self):
        self.age += 1
        print(f"Happy birthday, {self.name}! You are now {self.age} years old.")


# 創建 Person 類的實例
person1 = Person(name="Alice", age=30)

# 呼叫 greet 方法
print(person1.greet())  # 輸出: Hello, my name is Alice and I am 30 years old.

# 呼叫 haveBirthday 方法
person1.haveBirthday()  # 輸出: Happy birthday, Alice! You are now 31 years old.

# 再呼叫 greet 方法
print(person1.greet())  # 輸出: Hello, my name is Alice and I am 31 years old.

person2 = Person(name="Alan", age=20)

# 呼叫 greet 方法
print(person2.greet())  # 輸出: Hello, my name is Alice and I am 30 years old.

# 呼叫 haveBirthday 方法
person2.haveBirthday()  # 輸出: Happy birthday, Alice! You are now 31 years old.

# 再呼叫 greet 方法
print(person2.greet())  # 輸出: Hello, my name is Alice and I am 31 years old.
```
