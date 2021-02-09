# Git-TIL.md

# Reactチュートリアル
##Reactとは？
Reactとは宣言型のプログラミング言語で複雑なUIをいくつかの小さなコンポーネント組み合わせて作るもの。
jsxでコンポーネントを返す。コンポーネントは自分でも作れる。例えば<movie />など,,

<Square value{i} />はボタンの数
<button>
<this.props.value>
<btton/>で数を表示
reactはpropsで親から子に値を引き継ぐ
onClick => { alert('click)>}
アロー関数のほうが早い
Reactはstateを使ってっコンポーネントに学習させる
  
# ruby　チュートリアル

変数名は何の値が入れられているかわかりやすいやつにする
変数のいい例
name 
name_first アンダーバー良い
変数を作る理由
何度も同じことを書かなくても済む
値を変更しやすい

自信の変数を使って計算できる
number = nuber + 3
その場合
number+=3で省略できる
number * =3

## 変数展開
変数を文字列に組み込むときは変数展開を使おう
age = １９
puts  ”#{age｝歳です”
## if文　
if 条件
実行
ends

##比較演算子
a==b　aとｂは等しい
a!=b    aとｂは等しくない

## elseを使ったif文の型
if 条件
　　実行
else
　　実行

end

## rubyでのelse ifの書き方
elsif

## 条件の組み合わせ
「かつ」
  a>10 && b  <3

「または」

  a>10 || b  <3

## ruby 配列　
names ＝["nagaoka", shirakwa" , "tanaka"]
puts names
   で名前三つ出力

インデックス番号は0から始まる
また変数展開と配列の数字も組み合わせられる。
puts ’こんにちは#{name[1]’

## rubyチュートリアル
3**2 
**は二乗という意味。
Math.sqrt(9)
は平方根を研鑽してくれる。

defで関数を定義する
def  hi
puts "Hello World"
end
で”Hello World"が出力される。
### 特定の人の名前を入れたいとき
def hi(name)
と引数を置いて
puts "Hello #name}!"
end

hi("tarou")
で　Hello tatouと出る

class Greeter

def initialize   (name = world)
@name＝name 
end
def say_hi
  puts "Hello #{name}!"
end
def say_bye
puts "bye #{name}!"

nameがなかった場合hello worldになる。

greeterオブジェクトを作る
greeter = Gteeter.new(pat）で代入

## progate
配列.each do 変数
実行
end

変数ができる範囲をスコープと呼ぶ

変数の出力
put 変数
## ハッシュ
ハッシュとは配列とは違い、違う値を箱に入れること
変数　＝｛　キー　＝＞値、キー　＝＞値｝
puts 変数

困ったときはri
irbでは何かを試したい時にすぐ使えるので便利

## 複数行のコメント
=begin
あ
あ
あ
=end

## コマンド
print 
puts　　改行
p 　　　文字列（"")つけてくれる。
## オブジェクト
 "hello world"や1.1 などをオブジェクトという。
オブジェクトの後ろんいはメソッドという命令がつけれる。
"hello world".length→　文字列の数
　　　　　 .reverse→　文字列を逆順に返す
1.1floorなら小数点切り捨て
オブジェㇰトにも種類があり文字列の値を持つオブジェクトは
string class 
整数や小数点を持つ変数を
  float  class 
オブジェクトの値をinstanceと呼ぶ


## 定数
最初は英大文字
すべて大文字であることが多い。
途中で値を書き換えていけない。が値を変えても警告がでるだけで表示はされる。

## オブジェクト
"hello

rubyonrails 
rubyの表示は
controller 
view 
rooting
からできている。
rubyのviewまでの流れ
url→rooting→controller→view

rootingを変えるとurlも変えることができる。
get => home/top を get => top
するとURLも変わる。
stylesheet内のcssを変えると勝手にviewも変わる

puts "great" if score >80
といった書き方もできる

!=は等しくない。

## caseの条件分岐
case signal

when "red"
puts "warning"

when "yellow"
puts "caution"

when "blue"
puts "go!"

else 
puts "   wrong    signal


## 2/05 rails
get g controller コントローラー名　アクション名　

erbはrubyの拡張機能ファイル
変数を定義するときは
<%     値        %>
変数を表示する時は
<%=  値　%>
<% 
posts = {
"文字列１”、
”文字列２”
｝
%>

## 2/06

HTMLにeach文を使って配列を表示
<% 配列.each do |変数|
　　　　中身
<& end %>

アクションで定義した変数は@で表示する
アクションの
def 

end　内でview用の表示ができる。


データベースは表みたいなもの
列がコラム
行が

マイグレーションファイルはデータの変更を指示するファイル？
   rails   g model  Post   カラム名:text

rails db: migrate
でデータを反映させる。

Appricartionmodeが反映されたクラスをモデルという

postでインスタンスを作成するにはnewメソッドが必要
post.new(content:,,,)
インスタンスを保存するにはsaveメソッドが使える。
これはpostクラスにapplicationRecordを継承したからである。

post.firstでテーブルの最初のデーターをとりだることができる。
post1 =Post.fitst
post.content (データの内容を表示させる）
Post.all ですべての値取得
Post.all[0].content
1番目の内容を表示させる。
railsでaタグを書く時は<
<%= link_to(第一引数（表示させる文字）、第二引数（url)) %>

loop do  
p i
i += 1
end
でエンドレスに＋１される。
if文で
breakやnextを書くと、特定の数字で止まったり、スキップしたりする。

def  syaHi 
p "hi"
end
メソッド内で定義した変数はメソッド外では呼び出せない。
 def sayhi( name = "nagaoka" )
p "hi"　＃引数が与えられなかったらデフォルトの長岡がでる　
end

class User  #クラスの値の最初は必ず大文字

def sayhi
p 　"hi"
end

end

tom =User.new #これで変数にメソッドを使えるようにできる。
tom.sayhi

class User  #クラスの値の最初は必ず大文字

def initialize(name)
@name = name
end

def sayhi(name

puts 　"hi" #{@name}
end

end
tom =User.new 
tom.sayhi("nagaoka")

インスタンスの変数をかえたい、、
その場合はattr_acsesserを使う
name=>(値）　値をセットするためのコトをgetter
name               値に入りこむことをgetterという

クラスメソッド
 def self.info
puts 
end
User.info #呼び出し
 
クラス変数
@@でかく
定数はすべて大文字が推奨

class 子クラス　＜　親クラス　#敬称の書き方。

end

オーバーライド
親クラスのを書き換えことができる。

##2/09 　greeting
メソッドとは複数の処理をまとめること
def   greeting
  puts こんちわ
  puts こんばんわ
end
defとendの間の処理はインデント半角2文字分
greeting

引数は二つ入れれる。
def shoping(item,price)



