# 通过Bintray添加工程到maven和jcenter上需要注意的事项

1、要将上传上maven和jcenter上的工程中不用的资源文件，
包括图标等，不用的全部删掉，一方面减小引用文件的大小，
另外一方面避免引入到新工程中发生冲突。

2、如果已经上传一个版本到bintray上（比如1.0.0），那么下次修改后再上传的话，需要手动把版本号提高（比如1.0.1）
否则AS会编译报错，提示发生冲突。