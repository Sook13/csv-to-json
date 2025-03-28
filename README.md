# csv-to-json
项目描述: 这是一个简单的Python脚本工具，用于将CSV文件转换为JSON格式。该工具通过命令行参数接收输入文件名、输出文件名和其他相关参数，能够灵活处理CSV文件的不同格式和内容需求。

## 主要功能 
文件读取：支持自定义输入文件名，默认为data.csv。  
文件输出：支持自定义输出文件名，默认为输入文件的basename加上.json后缀。  
CSV分隔符：支持自定义CSV分隔符，默认为','  
列名选择：支持指定列名作为表头，默认为第一行。  
列选择：支持仅使用部分列。  
行选择：支持读取部分行或跳过部分行。  
列添加：支持向转换后的JSON数据中添加空列。  
数据输出：支持将转换后的JSON数据写入文件或打印到控制台。  
### 示例
```
usage: python csv2json.py [-h] [-S SEPARATOR] [-i] [-I INDEXLABEL]
                   [-u USECOLS [USECOLS ...]] [-n NAMES [NAMES ...]]
                   [-a APPEND [APPEND ...]] [-p]
                   [infile] [outfile]
```
infile输入文件名，默认：data. csv   
outfile输出文件名，默认值[infile_basename].json

```-S ```指定CSV分隔符为逗号。   
```-H ```指定使用第0行作为列名。   
```-c ```指定仅使用前5列。   
```-u ```指定仅使用column1。   
```-n ```指定列名替换为name1和name2。   
```-N ```指定读取100行。   
```-s ```指定跳过前2行。   
```-r ```指定仅保留第0、1、2行。   
```-a ```指定向输出中添加一个名为new_column的空列。   
```-p ```指定在完成后打印格式化数据。   

### 开发环境
Python 3.12.8
