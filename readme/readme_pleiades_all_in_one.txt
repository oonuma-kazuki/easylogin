=========================================================================================
Pleiades All in One Eclipse
-----------------------------------------------------------------------------------------
URL    : http://mergedoc.osdn.jp/
MAIL   : kashihara @ me.com
AUTHOR : Shinji Kashihara (cypher256)
=========================================================================================

Pleiades All in One は開発対象となる言語によりパッケージを選択できる日本語 Eclipse ディストリビュー
ションです。インストールはダウンロードしたファイルをダブルクリックして解凍するだけです。


ライセンス
=========================================================================================

Pleiades 本体は EPL です。その他のプラグイン、ソフトウェアについては、それに含まれるライセンスの
記述を参照してください。


履歴
=========================================================================================

2022-12.20230212

・修正: github#125 -Dosgi.requiredJavaVersion=11 → 17 戻し
・更新: Java、STS、Lombok、Pleiades 更新

2022-12.20230204

・修正: github#125 誤った eclipse.ini 設定を修正 (-Dosgi.requiredJavaVersion=17 → 11)

2022-12.20230124

・修正: github#124 Pleiades All in One 2022-12 が重い・遅い・フリーズする
・修正: Amateras Modeler の新規クラス・ダイアグラムが作成できないなど問題の暫定対応

2022-12.20221215

・更新: Platform、Python、PHP 版の Eclipse バージョン表記が 2023-03 になっていたのを修正
・追加: キーバインド WWD 行コメント (Ctrl + /)
・追加: Axis2 ツール・プラグイン (2022 初頭のプラグイン大量削除分の復帰)

2022-12.20221211

・更新: Eclipse 2022-12 対応
・追加: デフォルト設定 - サーバー定義に Tomcat 10.1 追加、tomcat/10 インストール追加
・変更: デフォルト設定 - 新規 Gradle プロジェクトを Tomcat 10.1 に変更 (javax.servlet → jakarta.servlet)
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ

2022-09.20221018

・変更: デフォルト設定 - .html の関連付けを WTP から WWD に変更
・追加: デフォルト設定 - .vue に WWD 関連付け追加
・追加: デフォルト設定 - .xlsx に Windows Excel 関連付け追加
・追加: デフォルト設定 - 一般 > ワークスペース : ネイティブ・フックまたはポーリングを使用してリフレッシュ ON
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ

2022-09.20220914

・更新: Eclipse 2022-09 対応
・追加: Java 19 Support for Eclipse 2022-09 (Java 19 は付属しない)
・変更: 新規 Gradle プロジェクト作成ウィザードの雛形を Servlet (javax) CRUD サンプルに変更
・削除: プラグイン削除 ANSI Escape in Console (Eclipse Platform に統合されたため)
・削除: プラグイン削除 JBoss m2e-apt (Eclipse m2e に統合されたため)
・変更: デフォルト設定 - Java > コンパイラー > メソッド・パラメーターの情報を保管 OFF → ON
・変更: デフォルト設定 - Java 版: プロジェクト・エクスプローラー > フィルターおよびカスタマイズ > EE 関連 OFF
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ

2022-06.20220619

・修正: github#110 pleiades-2022-06-java-win-64bit-jre_20220618.exeの自己解凍書庫実行時にエラー

2022-06.20220618

・更新: Eclipse 2022-06 GA 対応
・修正: github#107 "Pleiades [カスタム]"設定で、Javaソースコメントがフォーマット対象となる場合がある
・修正: 自動更新 OFF の自動デフォルト設定を再設定 (ベース JEE → Java 変更時のデグレード)
・修正: パフォーマンス問題で削除していた Ansi コンソール・プラグインを復活
・変更: Windows 版 Gradle Java Home 自動デフォルト設定 java/11 解除 (toolingapi が 7.4 で 17 対応したため)
・変更: デフォルト設定 - 更新ダイアログの「すでにインストールされている項目を隠す」ON → OFF
・変更: 設定 > Java EE (JET テンプレート関連) 非表示化
・変更: Java EE パースペクティブ廃止 (サーバー・ビューは Java パースペクティブ初期表示、DTP 廃止のため)
・変更: 新規 Gradle プロジェクトの Eclipse プロジェクトのエンコーディング初期設定 UTF-8 追加
・変更: JAVA_HOME 切り替えバッチの空白パス対応
・軽量化: dropins に含まれる各 doc プラグインを削除

2022-06.20220515

・更新: Eclipse 2022-06 M2 対応
・修正: github#105 m2e-wtpプラグインについて
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ
・変更: Windows Python 版の初回起動時に get-pip.py を実行するように設定
・変更: キーバインド衝突修正
　ズームイン/アウト (Ctrl+[+] / Ctrl+[-]) そのまま
　領域縮小/展開 (Ctrl+[+] / Ctrl+[-]) → (Ctrl+Shift+[+] / Ctrl+Shift+[-])

2022-06.20220505

・更新: Eclipse 2022-06 M1 対応
・追加: Windows 版の java ディレクトリに JAVA_HOME を切り替えできるバッチファイル追加
・追加: Windows 版の tomcat ディレクトリに 8080 ポートを kill するバッチファイル追加
・変更: Pleiades Java パースペクティブに Boot ダッシュボード追加
・変更: Enhanced Class Decompiler のデフォルト逆コンパイラーを FernFlower から CFR に変更
・変更: Spring Boot の application.properties 関連付け追加
・変更: Gradle プロジェクト作成時の Servlet プロジェクト・テンプレートをよりシンプルな最小構成に変更
・変更: 設定 > 実行/デバッグ > 起動 > 起動中に終了して起動: OFF → ON に変更
・変更: CSS の関連付けを WTP から Wild Web Developer の「汎用テキスト・エディター」に変更
・変更: Python 3 を Windows embeddable package (+ pip) に変更
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ
・軽量化: プラグインに含まれる Java ソースを削除
・軽量化: XDoclet プラグイン削除

2022-03.20220326

・変更: Java Full Edition に付属の Java 8 を Oracle 版から Adoptium 版に変更
・追加: Java 18 Support for Eclipse 2022-03 追加 (Java 18 は付属しない)
・更新: STS デッドロック解消版に更新 https://github.com/spring-projects/sts4/issues/729
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ
・軽量化: オリジナルに付属している JustJ JRE プラグインを削除
・軽量化: Java Full Edition の eclipse/jre ディレクトリを廃止し、-vm ../java/17/bin 指定に変更

2022-03.20220316

・バグ修正: Java のコンテンツ・アシストが動作しない問題に対応
・更新: 不要な .DS_Store ファイルを削除

2022-03.20220313

・更新: Eclipse 2022-03 対応
・変更: Windows 版 zip を自己解凍書庫に変更 (デフォルト解凍先 C:¥pleiades¥YYYY-MM)
・追加: SQL Editor プラグイン追加
・改善: WTP サーバー・ビューの起動アイコンがダークテーマの見た目で改善するように再ビルド
・更新: Pleiades 更新、各種プラグイン・ツールのバージョンアップ
・軽量化: PDE, DTP, Mylyn プラグイン削除 (jar 300 個 (1/3) 以上削減)
