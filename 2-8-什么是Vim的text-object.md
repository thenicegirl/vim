# 2-8-什么是Vim的text-object.md

## Text Object-文本对象

## 文本对象操作方式
**[number]<command>[text object]** 
- 解释:
- number,表示次数
- command,是命令，如d(elete),c(hange),y(ank),v(iew)
- text object ，是要操作的文本对象，比如单词w， 句子s, 段落p
- 举例
0. iw ,inner word;       aw , a word
1. caw ,删除当前单词并且进入编辑模式
2. 3daw, 删除3个单词
3. ci + "/)/]/}, 快速删除括号内的内容，并且进入编辑模式
4. ca + "/}/]/}, 快速删除括号以及里面的内容，并且进入编辑模式
5. vi + )...等符号，快速选中括号内的内容


***

**示例文本**

 import com.drew.lang.Rational;      
 import com
 import.exif.ExifSubIFDDirectory;      
 import drew.metadata.exif.GpsDirectory;      
 import com.china.bj.exceptions.XmssEmptyThumbnailException;      
 import com.china.bj.exceptions.XmssException;      
 import com.china.bj.exceptions.XmssInsertExifException;      
 import com.china.bj.utils.IPUtil;      
 import org.apache.commons.imaging.ImageReadException;      

 import org.apache.commons.imaging.ImageWriteException;      
 import org.apache.commons.imaging.common.bytesource.ByteSourceArray;      
 import org.apache.commons.imaging.formats.jpeg.JpegImageParser;      
 import org.apache.commons.imaging.formats.jpeg.exif.ExifRewriter;      

 import org.apache.commons.imaging.formats.tiff.TiffDirectory;      
 {
    1222,
    llajsdf
 
 } 
 import org.apache.commons.imaging.formats.tiff.TiffImageMetadata;      
 import org.apache.commons.imaging.formats.tiff.constants.ExifTagConstants    ;      

***
