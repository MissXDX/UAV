项目：homework
=====
一 函数：
--------
1. int dealSignal(const char *pFilePath, int signalID, OUT char **pOut)<br>
   此函数用来读取文本中的数据，待analyticData处理后，再将结果显示出来<br>
2. int analyticData(char *pData, OUT char **ppUAVID, OUT int *pCoor)<br>
   此函数用来处理dealSignal函数从文本中读出来的信息，然后讲处理结果返回<br>
二 测试：
-------
输入：<br>
plane1 1 1 1<br>
plane1 1 1 1 1 2 3<br>
plane1 2 3 4 1 1 1<br>
plane1 3 4 5 2 5 9<br>
plane1 5 9 14<br>
plane1 7 8 9 1 1 1<br>

查询消息ID 0，输出：plane1 0 1 1 1<br>
查询消息ID 2，输出：plane1 2 3 4 5<br>
查询消息ID 4，输出：Error: 4<br>
查询消息ID 5，输出：Error: 5<br>
查询消息ID 100， 输出：Cannot find 100
