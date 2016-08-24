# NHFFileUtils
<h2>介绍</h2>
<p>用于I/O常用方法</p>
<h2>安装</h2>
<ul>
<li>pod 'NHFFileUtils'</li>
<li>手动下载然后将文件夹拖至工程中即可</li>
</ul>
<h2>使用方法</h2>

+(NSString*)AppBasePath:(NSString*)pathtype;

/**
 *  获取app中document路径
 *
 *  @param filename
 *
 *  @return
 */
+(NSString*)AppBaseDocumentPath:(NSString*)filename;

/**
 *  获取app中resource路径
 *
 *  @param filename
 *
 *  @return
 */
+(NSString*)AppBaseResourcePath:(NSString*)filename;

/**
 *  测试某个目录是否存在
 *
 *  @return
 */
+ (BOOL)testDicExist:(NSString*)dicPath;

/**
 *  创建一个目录
 *
 *  @param dicPath 
 */
+ (void)createDic:(NSString*)dicPath;

/**
 *  删除文件夹及文件级内的文件
 *
 *  @param dicPath
 */
+ (void)deleteDicsAndFiles:(NSString*)dicPath;

/**
 *  拷贝一个目录到另外的一个地方
 *
 *  @param filePath
 *  @param toFilePath 
 */
+ (void)copyFile:(NSString*)filePath toFilePath:(NSString*)toFilePath;

/**
 *  获取文件名的扩展名
 *
 *  @param fileName
 *
 *  @return
 */
+ (NSString *)fileExtString:(NSString *)fileName;
