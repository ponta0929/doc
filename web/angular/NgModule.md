Angularのプロジェクトはルートモジュール1つと複数のモジュール群からなる

構文的には@NgModuleデコレータがついたクラスのこと
モジュールはアプリを開始する際か、ルータによって遅延ロードされる

○　@NgModuleで管理するメタデータ
    imports
        そのモジュールが依存しているモジュール群
    exports
        そのモジュールが提供する機能を定義する
    declarations
        そのモジュールで定義したコンポーネントやらディレクティブやらを書く場所



○　よく使われるモジュール
    BrowserModule
        @angular/platform-browser
        アプリケーションをブラウザで実行させるためのモジュール
        NgIfとかNgForも入ってる
        ルートモジュールに一度インポートされる
    CommonModule
        @angular/common
        NgIf, NgForを使うため
        フィーチャーモジュールの方でディレクティブだけ入れたいときとか使う
    FormsModule, ReactiveFormsModule
        @angular/forms
        ngModelとかフォームを良い感じに使うやつ
    RouterModule
        @angular/router
        ルーティング関連を行うため
    HttpClientModule
        @angular/common/http
        HTTP通信を行うため
    


