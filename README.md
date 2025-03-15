# 帧同步
`FrameBuffer` 帧缓存，其结构是一个环形缓冲区。作为临时数据存储，
|Fields|Description|
|:---|:---|
|`int MaxFrame`|指向缓冲区的末尾，初始值60|
|`List<OneFrameInputs> frameInputs`|输入缓冲，Capacity:120|
|`List<MemoryBuffer> snaphots`|快照缓冲，Capactiy:120|
|`List<string> hashs`||
# 服务器
为每个房间创建一个**纤程**，SceneType为`RoomRoot`
`Room`
