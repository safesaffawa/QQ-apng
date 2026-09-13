# 准备事项
1.准备**三个**图片(有示例文件)\
  以及仓库的1个apng间隔时间文件(文件名要与图片名一致)⚠️
  
  A图片为缩略图用来隐藏内容🤔\
  B图片为你想要放的内容😋\
  C图片为改了一个像素的B图片😋\
  防止apng自动合并图片
  
2.**检查B图片与C图片为PNG RGBA32格式**⚠️\
  来确保pc端不会自动播放apng
  
3.[**可选**] 使用**ffmpeg**来转码为RGBA32格式⚠️\
  ffmpeg -i input.png -pix_fmt rgba output.png
  
4.利用**apngasm**来将png图片合成为apng文件(x=png01)\
  apngasm output.png x.png 10 1 -f -l1

**apngasm**下载 https://sourceforge.net/projects/apngasm/files/2.91/apngasm-2.91-bin-win64.zip/download
