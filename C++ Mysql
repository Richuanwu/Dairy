# MySQL项目开发的一些记录 C++环境编程
1.从远端数据库的blob字段内容（假设存放了几百字节二进制的内容）取出到本地文件夹中：
istream *tmp;
tmp = ret->getBlob("/*字段名称*/");
istreambuf_iterator<char> isb = istreambuf_iterator<char> * tmp;
string blobstring = string(isb,istreambuf_iterator<char>());
ofstream FingerFeature;
FingerFeature.open(filestr,ios::binary);//filestr是文件存放名和文件类型，如“01.txt”
FingerFeature << blobstring;
FingerFeature.close();
