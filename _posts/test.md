| 字段           | 偏移量 | 字节数 | 含义                              |
| -------------- | ------ | ------ | --------------------------------- |
| BS_JmpBoot     | 0      | 3      | 跳转指令                          |
| BS_OEMName     | 3      | 8      | OEM名称                           |
| BS_OEMName     | 11     | 2      | 每扇区字数                        |
| BPB_SecPerClus | 13     | 1      | 每簇扇区数                        |
| BPB_RsvdSecCnt | 14     | 2      | 保留扇区数                        |
| BPB_NumFATs    | 16     | 1      | FAT个数                           |
| BPB_RootEntCnt | 17     | 2      | 根目录项数（FAT32已无该限制）     |
| BPB_TotSec16   | 19     | 2      | 扇区总数（小于32M使用）           |
| BPB_Media      | 21     | 1      | 存储介质描述                      |
| BPB_FATSz16    | 22     | 2      | 每FAT表占用扇区数 （小于32M使用） |
| BPB_SecPerTrk  | 24     | 2      | 逻辑每磁道扇区数                  |
| BPB_NumHeads   | 26     | 2      | 逻辑磁头数                        |
| BPB_HiddSec    | 28     | 4      | 系统隐含扇区数                    |
| BPB_TotSec32   | 32     | 4      | 扇区总数（大于32M使用）           |
| BPB_FATSz32    | 36     | 4      | 每FAT表扇区数（大于32M使用）      |
| BPB_ExtFlags   | 40     | 2      | 标记                              |
| BPB_FSVer      | 42     | 2      | 版本 (通常为0)                    |
| BPB_RootClus   | 44     | 4      | 根目录起始簇                      |
| BPB_FSInfo     | 48     | 2      | Boot占用扇区数                    |
| BPB_BkBootSec  | 50     | 2      | 备份引导扇区位置                  |
| BPB_Reserved   | 52     | 12     | 保留                              |
| BS_DrvNum      | 64     | 1      |                                   |
| BS_Reserved    | 65     | 1      | 保留                              |
| BS_BootSig     | 66     | 1      | 扩展引导标记                      |
| BS_VolID       | 67     | 4      | 序列号                            |
| BS_VolLab      | 71     | 11     | 卷标                              |
| BS_FilSysType  | 82     | 8      | 文件系统                          |