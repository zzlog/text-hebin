
# Account Data Merger

这是一个用于合并相同账号数据的 Python 脚本。

## 使用方法

1. 将你的数据保存到 `input.txt` 文件中，每行格式为：`账号,数据`。
2. 运行脚本：
   ```bash
   python main.py
合并后的数据将保存到 output.txt 文件中。

示例
输入文件 (input.txt)

acc1,data1

acc2,data2

acc1,data3

acc3,data4

acc2,data5

输出文件 (output.txt)

acc1,data1,data3

acc2,data2,data5

acc3,data4
