HTML5のvideoタグについて
http://www.htmq.com/html5/video.shtml

・動画ファイルの指定
src属性で指定するか、<source>タグで指定する
<source>タグを指定した場合、上から順に読み込み可能なファイルが再生される
<source src="sample.mp4">
<source src="sample.ogv">

・自動再生
autoplay属性をつけると自動で読み込んだ後再生される
<video src="sample.ogv" autoplay></video>

・自動読み込み
一般的なブラウザではpreload属性を指定しなくても動画はあらかじめ読み込まれる
preload="auto"
preload="metadata"
preload="none"
負荷的にはmetadataがベター？

・インターフェイス
controls属性を指定すると、ブラウザ標準のコントロール用のインターフェースが表示される
<video src="sample.ogv" controls></video>

・サムネ
poster属性で画像を指定する
<video src="sample.ogv" poster="firstframe.jpg"></video>

・その他
width属性：幅を指定する
height属性：高さを指定する