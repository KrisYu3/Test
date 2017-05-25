# VoiceConvert
提供Wav与Amr互转的接口,只需导入整个文件夹
导入头文件VoiceConvert.h
示例代码:
BOOL isConvert =  [VoiceConverter amrToWav:AMRFilePath wavSavePath:WAVFilePath];
        if (isConvert) {
            NSError *playerError;
            self.player = [[AVAudioPlayer alloc] initWithContentsOfURL:[[NSURL alloc] initFileURLWithPath:WAVFilePath]error:&playerError];
        }
需要分别提供被转换文件的地址和保存的地址
 
