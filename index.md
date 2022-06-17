---------------------------------------
---------------------------------------
---------------------------------------

# 伯牙（boya）AI音乐创作系统
## 和声感知的层次化音乐Transformer模型（Harmony-Aware Hierarchical Music Transformer-HAT, ACM MM reviewing）
<a href="https://arxiv.org/pdf/2109.06441.pdf">PDF</a>
<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/HAT.png" /> <br/>
1. 我们提出以和声为桥梁，联合学习乐曲的时间结构（曲式）和空间结构（纹理）。<br/>
2. 我们设计了一个端到端的和声感知的层次化音乐Transformer模型。<br/>
3. 我们开发了2个评价音乐结构性的客观指标体系。<br/>
4. 我们的模型可以大幅度的提升生成乐曲的曲式和纹理结构。<br/>
</div>


## 流行钢琴曲纯音乐（Pop-piano Music）生成能力
### 应用场景
1. 有作曲经验的用户，可指定和弦进行模板和律动模板，定制自己的AI乐曲。
2. 无作曲经验的用户，可指定场景、氛围、风格，定制自己的AI乐曲。
3. 该类型的乐曲，可以直接用于欣赏或是作为短视频的配乐。

### 核心方法
<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/pop.png" /> <br/>
整体流程包括：<br/>
<b>旋律创作</b>：算法模型根据用户的输入创作合适的旋律。<br/>
<b>伴奏创作</b>：算法模型旋律创作合适的钢琴伴奏。<br/>
<b>自动编排</b>：短乐段自动编排成长乐曲。<br/>
<b>自动混音</b>：平衡各分轨音量，添加混响效果。<br/>
</div>
<br/>

### 代表作品
<div style="border:1px solid green; text-align:center">
1.《锦时》
<audio controls="">
<source src="/music/resource/audio/lovely_ages.mp3" type="audio/mp3" />
</audio>
<br/>

2.《溪流》
<audio controls="">
<source src="/music/resource/audio/stream.mp3" type="audio/mp3" />
</audio>
<br/>

3.《暖冬》
<audio controls="">
<source src="/music/resource/audio/warm_winter.mp3" type="audio/mp3" />
</audio>
<br/>

4.《落雨的春天》
<audio controls="">
<source src="/music/resource/audio/raining _spring.mp3" type="audio/mp3" />
</audio>
</div>

---------------------------------------
---------------------------------------
---------------------------------------

## 史诗级音乐（Epic Music）生成能力

### 应用场景
1. 有作曲经验的用户，可指定和弦进行模板和律动模板，定制自己的AI乐曲。
2. 无作曲经验的用户，可指定场景、氛围、风格，定制自己的AI乐曲。
3. 该类型的乐曲，比较适合作为大场景的配乐，比如电影。

### 核心方法
<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/epic.png" /> <br/>
整体流程包括：<br/>
<b>旋律创作</b>：算法模型根据用户的输入创作合适的旋律。<br/>
<b>自动编曲</b>：为旋律自动配和弦、贝司、鼓组等轨道。<br/>
<b>自动编排</b>：短乐段自动编排成长乐曲。<br/>
<b>自动混音</b>：平衡各分轨音量，添加混响效果。<br/>
</div>

### 代表作品
<div style="border:1px solid green; text-align:center">
1.《奔腾》
<audio controls="">
<source src="/music/resource/audio/gallop.mp3" type="audio/mp3" />
</audio>
<br/>
 
2.《时间穿越》
<audio controls="">
<source src="/music/resource/audio/time_travel.mp3" type="audio/mp3" />
</audio>
<br/>

3.《向荣耀进发》
<audio controls="">
<source src="/music/resource/audio/head_for_glory.mp3" type="audio/mp3" />
</audio>
<br/>

</div>

---------------------------------------
---------------------------------------
---------------------------------------
## 根据用户哼唱的旋律，进行乐曲生成

### 应用场景

无作曲经验的用户，可以通过人声哼唱一段旋律，得到一首续写的乐曲。旨在降低用户的音乐技能门槛。

### 核心方法

<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/humming.jpeg" /> <br/>
整体流程包括：<br/>
<b>哼唱转录</b>：把用户的哼唱音频转录为乐谱。 <br/>
<b>前奏续写</b>：算法模型依次生成续写的律动和音高。 <br/>
<b>自动编曲</b>：为旋律自动配和弦、鼓组等轨道。 <br/>
<b>自动编排</b>：短乐段自动编排成长乐曲。 <br/>
<b>自动混音</b>：平衡各分轨音量，添加混响效果。 <br/>
</div>
<br/>

<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/humming_model.png" /> <br/>
生成算法模型：<br/>
<b>输入</b>：用户哼唱转录完的文件。 <br/>
<b>中间结果</b>：预测乐曲律动。 <br/>
<b>最终结果</b>：续写的旋律片段<br/>
</div>
 

### demo 1
<div style="border:1px solid green; text-align:center">
用户哼唱的音频:
<audio controls="">
<source src="/music/resource/audio/demo1-input.mp3" type="audio/mp3" />
</audio>

续写的乐曲:
<audio controls="">
<source src="/music/resource/audio/head_for_glory/demo1-0617.mp3" type="audio/mp3" />
</audio>
</div>

### demo2

<div style="border:1px solid green;text-align:center">
用户哼唱的音频:
<audio controls="">
<source src="/music/resource/audio/demo2-input.mp3" type="audio/mp3" />
</audio>
续写的乐曲:
<audio controls="">
<source src="/music/resource/audio/demo2-0617.mp3" type="audio/mp3" />
</audio>
</div>
---------------------------------------
---------------------------------------
---------------------------------------
## 人机协作的出版级音乐制作

### 应用场景

各项技术子能力，作为效率工具，与专业作曲人协同生产高质量出版级作品。

### 人机协同过程
<ol>
<li>人类作曲者给出基本的和弦行进框架。</li>
<li>算法生成旋律和伴奏。</li>
<li>填词。</li>
<li>现场录制。</li>
<li>后期：修音、混音、母带。</li>
<li>发行。</li>
</ol>

### 代表作品1：《2022微信公开课pro主题曲-入微》
<video width="" height="" controls>
<source src="/music/resource/video/ruwei.mov">
</video>

### 代表作品2：《2022腾讯志愿者之歌》
<video width="" height="" controls>
<source src="/music/resource/video/volunteer.mov">
</video>

---------------------------------------
---------------------------------------
---------------------------------------
## 更多作品欣赏，请关注 QQ音乐(<a href="https://y.qq.com/n/ryqq/singer/002dUuzA0FI573/album">耀灵</a>)、微信视频号WeAIArtist

---------------------------------------
---------------------------------------
---------------------------------------
## (附) 音乐理论基础

### 音阶、调式、和弦
<div>
<img src="/music/resource/image/Cmajor.jpeg" alt="音阶、音程、和弦、和弦功能和特性（以C大调为例）">  <br/>
<ol>
<li>现代音乐通常基于十二平均率理论基础，即以八度为一个循环，一个八度内包含12个音阶，对应钢琴的一组7白5黑琴键。音阶之间存在音程和度数差。</li>
<li>三个以上的具有度数差的音，同时演奏，构成和弦。</li>
<li>和弦本身带有自己的情感特性，和弦之间的转移进行，构成情感推进特性。</li>
<li>音乐的行进基本上是：制造不稳定状态 -> 回到稳定状态，称为从“待解决”到“解决”。和弦的转移进行路线，会指明乐曲的情感发展路线。</li>
</ol>
</div>


### 乐曲的结构性
<div >
<img src="/music/resource/image/overview.jpeg" alt="乐器的时空结构拆解"/><br/>

<ol>
<li>乐曲构成单元是<b>音符</b>，每个音符具有自己的<b>音高、音量、时值（长度）</b>。多个音符组成<b>和弦</b>。</li>
<li>乐曲有<b>全局属性</b>，包括：调式、拍号、速度等。</li>
<li>乐曲在时间维度上具有<b>曲式结构性</b>。从层次结构视角上看，以动机为起点，发展至乐节、乐句...直到乐曲。从功能逻辑视角上看，可分为前奏、主歌、桥段...尾奏等。</li>
<li>乐曲在空间维度上具有<b>声部结构性</b>，具体体现在多声部的行进关系上。</li>
<li>乐曲的整体风格加上演奏时的配器选择，产生不同<b>流派</b>的分野。</li>
</ol>

</div>
<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/score.png" /> <br/>
音乐结构性示例：一首完整时间结构（前奏、主歌、副歌、间奏、尾奏）的4轨道（主旋律、副旋律、和声、律动）乐曲。
</div>

### 乐曲的电子文档格式：midi文件
MIDI(Musical Instrument Digital Interface)乐器数字接口 ，是20 世纪80 年代初为解决电声乐器之间的通信问题而提出的。MIDI是编曲界最广泛的音乐标准格式，可称为“计算机能理解的乐谱”。它用音符的数字控制信号来记录音乐。一首完整的MIDI音乐只有几十KB大，而能包含数十条音乐轨道。几乎所有的现代音乐都是用MIDI加上音色库来制作合成的。MIDI 传输的不是声音信号， 而是音符、控制参数等指令, 它指示MIDI 设备要做什么，怎么做， 如演奏哪个音符、多大音量等。它们被统一表示成MIDI 消息(MIDI Message) 。传输时采用异步串行通信, 标准通信波特率为31.25×( 1±0.01) KBaud。（摘自 百度百科）


<div style="border:1px solid green; text-align:center">
<img src="/music/resource/image/midi.png" /> <br/>
图示为使用Apple Logicx打开的一个midi文件中的两个乐句。算法需要建模的就是这种音符序列规律。
</div>

