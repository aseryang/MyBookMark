【16进制转为字符串】
如 char buf[3] = {0x01, 0x02, 0x03} 转为 010203
void Hex2Str(unsigned char *sSrc, unsigned char *sDest, int nSrcLen ) 
{
	int i;
	char szTmp[4];
	for( i = 0; i < nSrcLen; i++ )
	{
		sprintf(szTmp, "%02X ", (unsigned char) sSrc[i]);
		memcpy( sDest + i * 3, szTmp, 3);
	}
	return;
}
【log4cpp使用】
http://blog.csdn.net/kingskyleader/article/details/7320826

【协议栈开发心得】
http://blog.csdn.net/findaway123/article/details/18097273
