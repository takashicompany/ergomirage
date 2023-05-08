# Ergomirage

<img src ="https://user-images.githubusercontent.com/4215759/236667857-117c0653-d2c5-4e63-bf0d-a06510bcd19d.png" width = "600px" />

Ergomirage(エルゴミラージュ)は、手配線のキーボードのような透明感をキットとして実現するべく設計されたキーボードです。

PCBの面積を極限まで減らし、透明なアクリルケースを用いることで、まるでキーだけが浮きがるような印象を醸し出します。

またキー配列も透明感を演出しつつも、実用性を踏まえたデザインとなっています。

## 部品

### キットに含まれているもの
|部品|個数|備考|
|:--|:--|:--|
|PCB|1||
|スイッチプレート|1|3mm厚アクリルプレート|
|ボトムプレート|1|3mm厚アクリルプレート|
|[ダイオード(表面実装型)](https://shop.yushakobo.jp/collections/all-keyboard-parts/products/a0800di-02-100)|44||
|[タクトスイッチ](https://akizukidenshi.com/catalog/g/gP-08081/)|1||
|ゴム足シール|8||
|ネジ(M2 5mm)|28||
|スペーサー(M2 5mm)|14||

### ご自身で用意頂くもの
|部品|個数|備考|
|:--|:--|:--|
|[Cherry MX互換キースイッチ](https://shop.yushakobo.jp/collections/all-switches)|44||
|キーキャップ|44|全て1uサイズ|
|[Pro Micro](https://talpkeyboard.net/?category_id=59e2ad48c8f22c3720001301)|1|動作確認済みのものは[こちら](https://talpkeyboard.net/items/62e24e6f8a0bd07fe2d38137)|

### お好みで
|部品|個数|備考|
|:--|:--|:--|
|[コンスルー](https://talpkeyboard.net/?category_id=5e451917cf327f255e6ae3ba)|2|Pro Microにハンダ付けを行うことでPCBとのハンダ付けが不要になります。Pro Microが壊れた際などに交換が容易になりますので、可能な限り取り付けをオススメします。|

### 1. PCBの表裏を確認する

表  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4451.jpg" width = "600px" />

裏  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4455.jpg" width = "600px" />

### 2. ダイオードの取り付け

各キースイッチの電流を通す・押下を検知するためにダイオードを取り付けます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4454.jpg" width = "600px" />

ダイオードのハンダ付け箇所の片側に事前にハンダを乗せておきます。(予備ハンダ)
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4455.jpg" width = "600px" />

ピンセットでダイオードを持ち、予備ハンダを溶かしながらダイオードの片側をハンダ付けします。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4456.jpg" width = "600px" />

もう片側もハンダ付けをして取り付け完了です。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4458.jpg" width = "600px" />

### 3. リセットスイッチの取り付け

リセットスイッチを取り付けます。リセットスイッチはPro Microにファームウェアを書き込む際などに書き込み状態にする役割などがあります。  
取り付け位置はPCB裏面の中央、ProMicro取付箇所の裏側です。  
ダイオードと同じ要領で一箇所のみ予備ハンダを行います。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4461.jpg" width = "600px" />

ダイオードと同様に、ピンセットでリセットスイッチを持ちながら予備ハンダを溶かして取り付けます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4462.jpg" width = "600px" />

残りの3箇所もハンダ付け行います。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4465.jpg" width = "600px" />

### 4. Pro Microの取り付け

Pro MicroをPCBに取り付けます。  
PCBとPro Microをピンヘッダでハンダ付けすることも可能ですが、慣れていない方はコンスルーを利用されると良いかと思います。  
コンスルーをPro Microにハンダ付けすることで、Pro MicroをPCBに挿し込むだけで使用することができます。  
Pro Microが壊れたりした際に取り替えが容易になりますので、コンスルーの使用を強く推奨します。  

コンスルー(ピンヘッダ)をPro Microにハンダ付けします。一般的なPro Microの場合、チップなどが載った面が下側になるように、コンスルー(ピンヘッダ)を配置しハンダ付けをします。Pro MicroとPCBのピン番号が合うかを確認してください。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4467.jpg" width = "600px" />

Pro Microの基板側から見たときの図。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4468.jpg" width = "600px" />

Pro MicroをPCBに取り付けます。PCBの表面にPro Microを差し込みます。Pro MicroとPCBのピン番号が合致していることを確認しながら取り付けてください。ピンヘッダの場合はPCBの裏面からピンヘッダをハンダ付けします。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4469.jpg" width = "600px" />

### 5. 各キーが動作しているかを確認する

Pro MicroにUSBケーブルを取り付けて、PCと接続します。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4479.jpg" width = "600px" />

[Remap](https://remap-keys.app/catalog/bOtvavSd8ne4UaCphfHA/firmware)からファームウェアを書き込みます。  

<img src = "https://user-images.githubusercontent.com/4215759/236870851-b60020ea-8255-4d1f-a633-fdc215bf73f0.png" width = "600px" />

RemapからVIA対応ファームウェアを書き込み後、RemapのTest Matrix Modeを開きます。  
<img src = "https://user-images.githubusercontent.com/4215759/235498918-e779201f-b11f-40db-ab1c-f4741852764c.png" width = "600px" />

Test Matrix Modeでは、キーが正しく入力されているかを確認することができます。
押したキーの箇所が点灯することを確認します。  
<img src = "https://user-images.githubusercontent.com/4215759/235499144-41df71d3-16b1-46a6-a719-8b7d3401c70b.png" width = "600px" />

ピンセット等でPCB裏面の各キースイッチのハンダ付け箇所を導通させることで、キースイッチをハンダ付けする前に各キーが正しく動作するかを確認できます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4481.jpg" width = "600px" />

全て点灯したら、ダイオードハンダ付けが問題なく行えていることとなります。  
仮に点灯しない箇所がありましたら、ダイオードのハンダ付けかPro MicroとPCBの接続が上手くいってないことが原因として考えられますので、確認をしてみてください。

### 6. キースイッチとスイッチプレートの取り付け

キースイッチをPCBに取り付けます。  

キースイッチプレートを取り出し、保護シートが貼ってある場合は両面ともに剥がします。  
剥がしづらい場合は、水を保護シートに含ませる・ピンセットなどで剥がすと良いかと思います。  
尚、製造の工程でアクリル板をカットした際に、一部に小さな指紋のような汚れがついてしまうことがございます。ご了承ください。
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4466.jpg" width = "600px" />

ご用意頂いたキースイッチをいくつか取り付けます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4478.jpg" width = "600px" />

キースイッチプレートにキースイッチを差し込みます。キースイッチプレートは表裏がございませんので、お好きな方を表としてお使いください。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4484.jpg" width = "600px" />

数個のキースイッチでスイッチプレートとPCBを仮組みをします。
キースイッチを数個程度キースイッチプレートに取り付けたら準備完了です。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4482.jpg" width = "600px" />

キースイッチがスイッチプレートから外れないように裏返し、PCBを載せます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4485.jpg" width = "600px" />

PCBの裏面からキースイッチの足が出ていることを確認し、ハンダ付けを行います。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4486.jpg" width = "600px" />

仮組み用のキースイッチのハンダ付けが終わったら、表面にしてスイッチプレートが固定されていることを確認します。  
慣れていない方は、各キースイッチが動作するかを確認すると着実に完成に近づきます。
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4487.jpg" width = "600px" />

残りのキースイッチをスイッチプレートに取り付けます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4489.jpg" width = "600px" />

仮組みと同様に各キースイッチから足が出ているかを確認し、問題なければハンダ付けを行います。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4490.jpg" width = "600px" />

全てのスイッチをハンダ付けした後に、再度Pro MicroとPCをUSBケーブルで繋ぎ、全てのキースイッチが動作することを確認すると手戻りが少なくなるかと思います。

### 7. ボトムプレートの取り付け

ボトムプレートを取り出します。スイッチプレートと同様に保護シートが貼られている場合は剥がしてください。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4492.jpg" width = "600px" />

スペーサーとネジでスイッチプレートとボトムプレートを固定します。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4493.jpg" width = "600px" />

スイッチプレートを裏返して、ネジとスペーサーを内側(キースイッチの十字とは逆の向き)に取り付けます。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4494.jpg" width = "600px" />

スイッチプレート全ての穴にネジとスペーサーを取り付けます。全部で14箇所になります。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

ボトムプレートを先程取り付けスペーサーに載せ、ネジで固定します。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4498.jpg" width = "600px" />

### 8. ゴム足シールの取り付け

ゴム足シールをお好きな箇所に貼り付けます。  
<img src = "https://github.com/takashicompany/minidivide/raw/master/images/build/IMG_3748.jpg?raw=true" width = "600px" />

### 9. キーキャップを取り付ける

最後にキーキャップを取り付けて完成です。  
<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_4499.jpg" width = "600px" />

<!---

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />

<img src = "https://raw.githubusercontent.com/takashicompany/ergomirage/master/images/build/IMG_.jpg" width = "600px" />


--->
