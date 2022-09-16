# 4入力ステレオミキサー ビルドガイド
- [ご注意](#ご注意)
- [部品リスト](#部品リスト)
- [組み立て](#組み立て)
- [おまけ](#おまけ)

## ご注意
- Type-A to Type-Cケーブルでのみ給電できます。
- ボリューム調整機能はありません。
- マイクには対応していません。
- 入力端子同士の間隔は1.2cmです。

## 部品リスト
![](img/IMG_9521.jpeg)  
|Ref|部品名|数|
|-|-|-|
||メインボード||
||アクリルプレート||
||0.01mm両面テープ||
||5mmM2ねじ|8|
||3x8mmスペーサー|4|
|U1|丸ピンICソケット 14P|1|
||オペアンプ LME49740NA|1|
|MAU108|レギュレーター MAU108|1|
|REG1|レギュレーター NJM7805FA|1|
|USB1|Type-Cコネクタ電源供給用|1|
|TRRS1-5|MJ-4PP-9|5|
|R1-10|47kΩ|10|
|R11-16|10kΩ|6|ｔ
|-|-|
|はんだ付け用工具一式||
|精密ドライバー||
|ニッパー|抵抗等の足を切ります。|
|ラジオペンチ|レギュレーターの足を曲げます。ニッパーでも可能です。|
|アクリサンデー ポリケアF70|指紋を拭いたりホコリを付きにくくできます。|
|アクリサンデー 研磨剤|側面を磨いてツルツルにしたり、細かい傷を消すことができます。|
|アクリル接着剤|両面テープの代わりに使うと強固に接着できます。|

## 組み立て
電子部品は番号通りに部品をはんだ付けするだけなのでビルドガイドを見なくても制作可能です。高さが低い順番にはんだ付けする様子を写真で紹介しています。  

![](img/IMG_8893.jpeg)  
![](img/IMG_8897.jpeg)  
Type-Cコネクタはマスキングテープなどで固定するとはんだ付けしやすいです。
![](img/IMG_8900.jpeg)  
![](img/IMG_8905.jpeg)  
![](img/IMG_8906.jpeg)  
OS-CONには極性があります。足が長い方が+（白い側）です。  
![](img/IMG_8908.jpeg)  
レギュレーターの足をラジオペンチ等で曲げます。
![](img/IMG_8909.jpeg)  
![](img/IMG_8910.jpeg)  
コイルや抵抗は写真のように足を曲げて縦に取り付けます。
![](img/IMG_8911.jpeg)  
![](img/IMG_8912.jpeg)  
![](img/IMG_8913.jpeg)  
![](img/IMG_8914.jpeg)  
![](img/IMG_8915.jpeg)  
![](img/IMG_8917.jpeg)  
![](img/IMG_8919.jpeg)  
![](img/IMG_8921.jpeg)  
フィルムコンデンサーには極性がありません。
![](img/IMG_8922.jpeg)  
電源用電解コンデンサーには極性があります。
![](img/IMG_8923.jpeg)  
オーディオ用コンデンサーには極性がありません。
![](img/IMG_8924.jpeg)  
![](img/IMG_8925.jpeg)  
すべてのパーツをはんだ付けしたらオペアンプを差し込んで動作を確認しましょう。
![](img/IMG_8930.jpeg)  

アクリルケースを組み立てます。スペーサー4つをネジで取り付けます。
![](img/IMG_9523.jpeg)  

アクリルプレートから保護フィルムを剥がしのせていきます。順番は写真を参考にしてください。
![](img/IMG_9524.jpeg)  
![](img/IMG_9526.jpeg)  
![](img/IMG_9527.jpeg)  
![](img/IMG_9529.jpeg)  
ネジは締めきらず、微調整できるようにしておくと側面を綺麗に揃えやすいです。  
  
裏返して片面を剥がした両面テープを貼ります。皮脂が付いていると剥がれやすくなるので気をつけてください。  
![](img/IMG_9533.jpeg)  

両面テープをはがし、側面のカーブを合わせて貼り付けます。
![](img/IMG_9535.jpeg)  
残りのプレートも同じように貼り付けます。
![](img/IMG_9536.jpeg)  
![](img/IMG_9538.jpeg)  
好みのキースイッチを差し込んで、ゴム足とキーキャップを付けたら完成です。 
![](img/IMG_9540.jpeg)  
![](img/IMG_9542.jpeg)  
![](img/IMG_9808.jpg) 


## おまけ
### LEDを光らせる
キースイッチによってはLEDを取り付ける穴が開いていないことがあります。また、LEDをはんだ付けするとキースイッチを外せなくなります。  
裏面のネジを外してプレートを取り除き、キースイッチの上からLEDを差します。写真と同じように、長い方の足が四角のパッドから出るようにしてください。  
![](img/IMG_9805.jpeg)  
![](img/IMG_9547.jpeg)  
はんだ付けして足を切り、プレートを戻します。
![](img/IMG_9548.jpeg)  
USBを繋いでスイッチを押すとLEDが発光します。

### ノイズ対策
ジリジリしたノイズが乗っている場合、グラウンドループアイソレーターを使うことで解決することがあります。
おまけの基板に別売りのTRRSジャック（[MJ-4PP-9](https://akizukidenshi.com/catalog/g/gC-06070/)）とトランス（[AT129](https://akizukidenshi.com/catalog/g/gP-14522/)）をはんだ付けすると作ることができます。
![](img/IMG_8887.jpeg)  
![](img/IMG_8891.jpeg)  
検索すると市販のものもたくさん出てくるので好きなものを使ってください。

### 自分で発注する
#### PCB
- [kicadファイル](https://github.com/Taro-Hayashi/4-input-stereo-mixer/releases/download/pcbandacrylic/mixer_pcb.zip)
- [Elecrow向けガーバー](https://github.com/Taro-Hayashi/4-input-stereo-mixer/releases/download/pcbandacrylic/mixer_80x70.zip)
#### アクリル
- [kicadファイル](https://github.com/Taro-Hayashi/4-input-stereo-mixer/releases/download/pcbandacrylic/mixer_acrylic.zip
- [Elecrow向けzipファイル](https://github.com/Taro-Hayashi/4-input-stereo-mixer/releases/download/pcbandacrylic/mixer_3mm_183x169.zip)
## 販売ページ
遊舎工房フリマで販売予定です。
- [BOOTH](https://tarohayashi.booth.pm/items/4144494)  
