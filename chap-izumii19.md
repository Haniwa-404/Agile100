﻿# わからないことだらけの世界を生きていく


<div class="flushright">伊藤 いづみ(@izumii19)</div>


## まえがき


システム開発をしているとたくさんのわからないことに出会いませんか？
不具合の原因がわからない、お客様やチーム内でのコミュニケーションがわからない、さらにはわからないことがわからないなど、「システム開発は"わからない"を"わかる"にしていく作業である」といってもいいくらいたくさんのわからないことがあります。


またアジャイルマニフェストの12の原則にはこのような一文があります。


>**Welcome changing requirements, even late in development.** Agile processes harness change for the customer's competitive advantage.

>**要求の変更はたとえ開発の後期であっても歓迎します。** 変化を味方につけることによって、お客様の競争力を引き上げます。


ここからはシステム開発が常に変化し続けるものであることがわかりますが、変化というのも「新たなわからないことの一つ」と考えることができます。


今回は私がこれまでの様々な経験から見えてきた、わからないこととうまく付き合う方法をお話したいと思います。


## わからないことは永遠になくならない
「わからないことを避ける」のではなく「付き合う」という考え方に至ったのは、私のシングルマザーとしての経験が実は大きく影響しているなぁと思います。


結婚して子供が生まれた時には、まさか自分がシングルマザーになってこのような人生を歩むことになるなんて想像もしませんでしたし、子供が何歳になったらパートに出て、毎年このくらい貯金して、何年後にはマイホームを建てて…と計画したことを堅実に遂行していくほうが安心するタイプの人間でした。


ですがふりかえってみると私の現実は何もかも想定外。生活のため予定よりだいぶ早くフルタイムワーカーとして働くことになり、同時に怒涛のワンオペ育児。貯金するほどの余裕もなく新築も新車も一人の稼ぎでは無理と早々断念しました。ほんとに全く想定外の人生、彦麻呂のネタを借りるならまさに「unknownの玉手箱や〜」です。


私はこの経験を通じて生きているかぎり想定外のことは無限におき続けるということを強く感じました。
未来は無限、だからこそわからないことも無限に起きます。そしてこれをコントロールすることは不可能ですから私達はただ受け入れるだけです。ですから未来に備えてチマチマと計画することやわからないことを避けることではなく、わからないことに対して上手に受け身をとり付き合っていくことが私達には必要なのではという考えに至りました。




## わからないことと付き合うには


今日は過去のWebエンジニアとして働いていた頃のお話をします。

Webエンジニアとして初めて携わったのが「Amazon DynamoDBから特定のデータを取得し、フロント側に返すAPIをDjangoを使って作る」という業務でした。みなさんにとってはなんてことないミッションかもしれませんが、当時の私はWebAPI開発経験なし、DynamoDBの知識なし、Python+Djangoも未経験。まわりに助けてくれる人がいないわけではないのですが、この時は入社したてで社内のコミュニケーションフローもよくわからない状態だったし、他メンバーも案件を抱えているため基本的に自分自身でなんとかしていく必要がありました。プロジェクトの期間もそれほど長くなく納期のプレッシャーもありました。

この状態で正直何から手をつけていいかもわかりませんでした。ただただモヤモヤとした不安な気持ちだけはずっとありました。この苦しい状態からなんとか脱出したいと思いやってみたことをこの後に書いていきます。


### 不安という感情によって自分自身を潰さない


わからないことと出会った時のみなさんの反応はどんな感じでしょう。ワクワクしますか？それとも不安でしょうか。
私は「何がなんだかわからない」のような漠然とした状態の時ほど不安が強くなります。単純なことが重大な事のように思えたり、本質を捉えることができずに見当違いな対応をしてしまい問題を余計に複雑にしてしまうなど、悲観的になったりテンパったりしてそれが結果として失敗につながってしまったような気がします。


脳科学者の中野信子さんによると[^nakano]日本人はもともと不安を感じやすい民族なのだそうで、これにはセロトニントランスポーターという遺伝子が関係しています。
セロトニントランスポーターには不安を感じやすい「SS型」楽観的な「LL型」、その中間の「SL型」という３つの型があるのですが、このうち日本人の7割弱が不安を感じやすいSS型なのだそうです[^ll]。

[^nakano]: 2020/11/5 ビジネスEXPOでの脳科学者中野信子氏によるセッション「コロナ禍のビジネスマンへ送るメッセージ〜不安な気持ちの中で“成功へ導く”考え方〜」のご講演内容より

[^ll]: ：ちなみに楽観的なLL型の遺伝子を持っている日本人はたった2%程度しかいないとか。

つまり、私達がわからないことや予期せぬ出来事が起こったときにワクワクより不安を感じやすいのは遺伝的のせいと考えることができます。

私はこの話を聞いてから、漠然とした不安が襲ってくると「この感情は遺伝子のせいで私の性格や準備不足のせいじゃない」といい聞かせて思い直すようにしました。
事実と感情を分離することにより不安という感情に自分自身のコントロールを乗っ取られることが少なくなりました。そして事実だけを俯瞰して観察できるようになりました。


### わからないことが何かを認知する
前述したような考え方でネガティブな感情を切り離したら、漠然とわからないことを「自分がわかっていること」とという視点に置き換えてみます。


* APIってどうやって作るのかわからない、ということがわかっている
* pythonがわからない、ということがわかっている
* Djangoがわからない、ということがわかっている
* DynamoDBがわからない、ということがわかっている




ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる


なにがなんだかわからないという状態を「私は自分のわからないことがわかっている」という自己認知の視点に切り替えることで、わからないことは何か浮き彫りにすることができます。漠然とした不安をもたらすものの正体が見えてくるので、この時点で不安な気持ちはだいぶ少なくなってきます。




### わからないことの解像度をあげる
次にわからないことの解像度をあげていきます。たとえば「pythonやDjangoわからない」については「本当に何もわからないんだっけ？」と自問しながら深掘っていきます。


* forやifなど処理の文法は、どの言語もたいしてかわらないだろうから実はなんとかなる
* python特有の書き方はわからないけどググってコピペでいけそう
* pythonからDynamoDBに接続する方法は全くわからない
* Webアプリケーションのフレームワークについては全然知識がない


ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる
ここに↑を表現する図をいれる




こうして分類していくと実はpythonそのものについては実はあまり不安はなく、初めてというだけで不安を抱えていたに過ぎませんでした。逆にDynamoDBやDjangoについては本当に何も知らないということがわかってきたので何か策を考える必要がありそうです。こうしてわからないことから「事実のunknown」と「妄想のunknown」を分別していきます。




### わからないことをわかるようにするアクションを考える
ここまでくると「わからないけど解決する必要があるもの」だけがふるいにかけれられて残っています。わからないことを解決するために自分が取れる具体的なアクションを考えていきます。


↓ここは図で表現する
* pythonからDynamoDBに接続する方法がわかるためには
   * DynamoDBについてまず理解する
      * ネット、AWS公式で調べる
   * pythonからDynamoDBに接続する方法について理解する
      * Qiitaや技術ブロクを使って調べる
      * 誰かに聞く
         * 自分が理解したい答えを明確にする
         * そのためになにを質問すればよいか考える
         * わかりそうな人を探す
   * わかったら試す
   * 知っている人に丸投げ


こうしてみると調べる・探す・聞くなど、アクションとしては単純なものばかりですからかなりハードルが下がりました。なんかやれそうです。


アクションを起こした結果「自分で調べたけど結局わからなかった」ということもありますが、そしたらまた「自分で調べるだけでは解決できなかった、ということがわかった」という状態を自己認知しわからないことの解像度をあげ、アクションを考え行動する、というのをくりかえします。


## わからないことと共存するということ
ここまでをまとめると、「わからないことと共存しうまく付き合うプロセス」は以下の通りです。


1. 不安を感じるのは遺伝子のせいと捉え、ネガティブな感情は切り離す
2. 自己認知の視点で、わからないことがわかっているということを認知する
3. わからないことに対し、事実と妄想を分別する
4. 「事実のunknown」に対し自分のとれるアクションを考え実施する




もしこの先、わからないことに出会い漠然とした不安を感じたときこそこの４ステップを試してみてください。不安というネガティブな感情が「なんとかなるかも」というポジティブな感情へなだらかに変化していくのを感じられるかと思います。


私はわからないことが多いほど誰かがやってくれるかもとか、なにかの間違いじゃないかとか、やらずに済む方向考えてしまいがちだったのでした。ですがこの逃避型の考え方は自身の行動に直結しづらく、行動なきところにはたいした変化も起きませんでした。やはり全ては自分ごととして捉え行動することに尽きるのだと思います。


そのためにまず湧き上がる不安という感情は全て遺伝子のせいにして、素の自分を取り戻すことから始めましょう。
そして「自分の想定外のことが今起きている。でもこのままではずっとこのままだ。」という事実を拒否せずに受け入れて見て下さい。その次にあなたはきっと何か行動を起こしているでしょう。


私の人生は「もう少し早くこのことに気付けていたら自分の人生は違ったんじゃないか」という後悔ばかりです。ですが、私の経験が未来あるみなさんの小さなヒントになればとても嬉しいです。