```c
// 世界は濁っているが、私は純粋だ。
byte world = 0b11111111;
byte me    = ~world;
printf("%d", me & world);
```

こんにちは、かざま ちづる。ブログでは九条詩織（くじょう しおり）、ID は KujouShiori —— 名前は二つありますが同じ人です。PC ゲーマー / 名古屋大学卒 / ことし京都大学の大学院に入った新入生、いまは研究室配属。歴史（卒论は日本古代史、今は日本近代史、神話史もかじってる）とコンピュータの二刀流。
2021 年から GitHub にいて、リポジトリ 33 個・star を 440 個押してきました。

- 🎮 シニア Steam プレーヤー | SteamID 899140041 | フレンド申請大歓迎
- 📍 愛知県名古屋市千種区栄町 〒464-8601 / 京都市左京区吉田本町 〒606-8501
- 🥚 このリポジトリにもう 1 つファイルがあるの、気づける？

### いま作っているもの

**Token 计岛（token-meter）** —— C#/.NET 製、WinIsland / WinLand（Windows 11 版ダイナミックアイランド）用プラグイン。
手元の AI クライアント会話ログと各社クラウド用量 API を叩いて、token 消費量・推定費用・残高・直近 7 日の推移を島に常駐表示します。単価は全部自分で設定でき、予算超過と残少は警告を出します。
一番気を使ったのは「足さない」こと。手元ログとクラウド API は運営元も通貨も違う別の帳簿なので、合算せず出典ごとに別行へ。落ちたら静かにローカルログへ退避します。API キーはプラグインにも settings.json にも置かず、環境変数名だけ持ちます。

- [luolangaga/WinLandPlugin](https://github.com/luolangaga/WinLandPlugin) のマーケット投稿：1.0.0 / 1.1.0 はマージ済み、1.2.0 は審査中

### 作っているもの / 集めているもの

| リポジトリ | なに |
| --- | --- |
| [Playersuite](https://github.com/KujouShiori/Playersuite) | Java —— NeoForge 1.21.1、遊びながら欲しいと思った機能を詰め込んだ MOD |
| [One_Piece_For_Minecraft](https://github.com/KujouShiori/One_Piece_For_Minecraft) | Java —— Bukkit 1.20+、BAN されたプレイヤーの遺産をどう始末するかというプラグイン |
| [UUIDManagerPlugin](https://github.com/KujouShiori/UUIDManagerPlugin) | Java —— 肌サイトに移行したとき、旧 offline ログインの uuid.dat を自動リネーム |
| [LocalFictionReading_UWP](https://github.com/KujouShiori/LocalFictionReading_UWP) | C# / UWP —— 手元の小説を読むだけのリーダー |
| [Minecraft-mod-sinicization](https://github.com/KujouShiori/Minecraft-mod-sinicization) | 自分が遊ぶ範囲の MOD 中国語化辞書。新版の訳を旧版に落とし込むのにも使う |
| [The-Elder-Scrolls-5-Skyrim-All-books](https://github.com/KujouShiori/The-Elder-Scrolls-5-Skyrim-All-books) | ★5 —— 天际の内置書籍を全部抜いた資料庫 |

遊びたいゲームに中国語がないので翻訳を始めた、というのがいちばん動機に近い。Minecraft / Galge / VN のローカライズと、消えたら困る資料のアーカイブが仓库の大半を占めます。ゲームのデータベースサイト（MirrorStation、BurstWitchCodex など）も自分で組んで GitHub Pages に置いてます。
もうひとつの軸はバイナリ。汉化するにはリソースの形式を読むしかない —— モバイル版の Lua リソースの暗号を、暗文统计から機械語特定、全ファイル再暗号化一致まで通して解析したけど、まだ公開してません。
他人のリポジトリに直接入れたのは [icey9527/Verviewer](https://github.com/icey9527/Verviewer) の PSD プレビューと汎用位置決め（8 commits）。Issue は 34 件（22 件クローズ）、ランチャー・MOD・デスクトップツールを問わず壊れてるものは勝手に報告します。

### 🛠️ Stack

![C#/.NET](https://img.shields.io/badge/C%23%2F.NET-512BD4?style=for-the-badge&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Assembly](https://img.shields.io/badge/Assembly-6E4C13?style=for-the-badge&logo=assemblyscript&logoColor=white)
![Windows 11](https://img.shields.io/badge/Windows%2011-0079d5?style=for-the-badge&logo=windows11&logoColor=white)
![NeoForge / Fabric / Bukkit](https://img.shields.io/badge/NeoForge%2FFabric%2FBukkit-00A85F?style=for-the-badge&logo=minecraft&logoColor=white)
![UWP / WPF](https://img.shields.io/badge/UWP%2FWPF-76D976?style=for-the-badge&logo=windows&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-0078d7?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

<p align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=KujouShiori&show_icons=true&theme=tokyonight&hide_border=true&bg_color=00000000"/>
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=KujouShiori&layout=compact&theme=tokyonight&hide_border=true&bg_color=00000000"/>
  <img src="https://komarev.com/ghpvc/?username=KujouShiori&color=0079d5&style=for-the-badge"/>
</p>

> 遊びに来たついでに、Steam のフレンド申請も待ってる。:-)
