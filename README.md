# generateJsonToJavaBean

- 根据接口自动生成 java bean

```shell
generate_java.py --h
usage: generate_java.py [-h]
                        [--json CONTENT]
                        [--className CLASSNAME]
                        [--outPath OUTPATH]
                        [--package PACKAGE]
                        [--outType OUTTYPE]

optional arguments:
  -h, --help            show this help message and exit
  --url URL             parsed json url [disabled]
  --json jsonContent    parsed json content
  --className CLASSNAME
                        specify root class name
  --outPath OUTPATH     Automatic generation of storage file path ,default
                        current path.
  --package PACKAGE     Generating the .java file class package name
  --outType OUTTYPE     1: parser 2:Gson
```

- 实例

```shell
[disabled] generate_java.py --url "http://api.budejie.com/api/api_open.php?market=360zhushou&order=repost&maxid=&udid=A0000044BEC447&a=list&c=data&os=4.2.2&client=android&page=1&per=10&visiting=&type=&time=week&mac=40%3A0E%3A85%3A1D%3A43%3AAE&ver=4.2.3" --className Test

generate_java.py --json "{}" --className Test

or

./json2bean jsonFile Test
```