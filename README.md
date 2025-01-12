﻿# wxp Project
from music21 import converter

# 导入 MusicXML 文件
# 请将 'path/to/your/musicxml/file.xml' 替换为实际的 MusicXML 文件路径
file_path = 'path/to/your/musicxml/file.xml'

try:
    # 使用 music21 的 converter 模块解析 MusicXML 文件
    score = converter.parse(file_path)
    
    # 如果解析成功，打印“成功”
    print("成功")
    
except Exception as e:
    # 如果解析失败，捕获异常并打印错误信息
    print(f"解析失败: {e}")
