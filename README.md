```c
// 世界は濁っているが、私は純粋だ。
byte world = 0b11111111;
byte me    = ~world;
printf("%d", me & world);
```

こんにちは、九条詩織（くじょう しおり）と申しますわ。ID の KujouShiori は、そのままこの名前の読み方なのよ。

わたしは PC ゲーマーで、名古屋大学を卒業して、ことし京都大学の大学院に入った新入生なの。いまは研究室に配属されておりますわ。歴史（卒論は日本古代史、いまは日本近代史、神話史もちょっとかじってるのよ）とコンピュータの二刀流をやってます♪
2021 年から GitHub にいまして、リポジトリは 33 個、star は 440 個も押させてもらったわ。

- 🎮 シニア Steam プレーヤーですわ | SteamID 899140041 | フレンド申請、大歓迎よ♪
- 📍 住所は二つありますわ：愛知県名古屋市千種区不老町 〒464-8601 / 京都市左京区吉田本町 〒606-8501
- 🥚 このリポジトリにもうひとつファイルを置いてあるの。見つかるかしら、たのしみ。

### いま作ってるもの

**Token 计岛（token-meter）** —— C#/.NET で、WinIsland / WinLand（Windows 11 版ダイナミックアイランド）用のプラグインを作ってるの。
手元の AI クライアント会話ログと各社クラウド用量 API を叩いて、token 消費量・推定費用・残高・直近 7 日の推移を島に常駐表示させますわ。単価は全部自分で設定できるようにしてあるのよ、予算を超えたら、残高が少なくなったら、警告も出てくるわ。
ここで一番気をつかったのは「足さない」ことなの。手元ログとクラウド API は運営元も通貨もちがう別の帳簿ですもの、合算なんてしたくないの。出典ごとに別行へ、落ちたら静かにローカルログへ退避します。API キーはプラグインにも settings.json にも置かなくて、環境変数の名前だけを持つようにしてるのよ♪

- [luolangaga/WinLandPlugin](https://github.com/luolangaga/WinLandPlugin) のマーケット投稿：1.0.0 と 1.1.0 はマージしていただいたわ、1.2.0 は審査中。

### 作ってるもの / 集めてるもの

| リポジトリ | なに |
| --- | --- |
| [Playersuite](https://github.com/KujouShiori/Playersuite) | Java —— NeoForge 1.21.1、遊びながら「これ欲しいな」と思った機能を詰め込んだ MOD |
| [One_Piece_For_Minecraft](https://github.com/KujouShiori/One_Piece_For_Minecraft) | Java —— Bukkit 1.20+、BAN されたプレイヤーの遺産をどう始末するかというプラグインよ |
| [UUIDManagerPlugin](https://github.com/KujouShiori/UUIDManagerPlugin) | Java —— スキンサイトに乗り換えたとき、旧 offline ログインの uuid.dat を自動リネームするの |
| [LocalFictionReading_UWP](https://github.com/KujouShiori/LocalFictionReading_UWP) | C# / UWP —— 手元の小説を読むだけのリーダーなの |
| [Minecraft-mod-sinicization](https://github.com/KujouShiori/Minecraft-mod-sinicization) | 自分が遊ぶ範囲の MOD 中国語化辞書。新版の訳を旧版に落とし込むのにも使ってるわ |
| [The-Elder-Scrolls-5-Skyrim-All-books](https://github.com/KujouShiori/The-Elder-Scrolls-5-Skyrim-All-books) | ★5 —— 天际のゲーム内書籍を全部抜いた資料庫よ |

もともと遊びたいゲームに中国語がなかったんですもの、それで翻訳を始めた、というのがいちばん動機に近いの。Minecraft / galgame のローカライズと、消えたら困る資料のアーカイブで仓库の大半が埋まってるわ。ゲームのデータベースサイト（MirrorStation、BurstWitchCodex など）も自分で組んで GitHub Pages に置いてますの♪
もうひとつの軸はバイナリよ。汉化したければリソースの形式を読むしかないわけで —— スマホのゲームの Lua をこっそり読み出せたときの喜びったらなかったわ、ちゃんと全ファイルで往復確認してから喜んでいるのよ。中身は、まだ公開してませんの。
他人のリポジトリに直接入れたのは [icey9527/Verviewer](https://github.com/icey9527/Verviewer) の PSD プレビューと汎用位置決め（8 commits）よ。Issue は 34 件（22 件クローズ）、ランチャーでも MOD でもデスクトップツールでも、壊れてるものはつい報告してしまう性分なの♪

### 🛠️ わたしの道具箱

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

> 遊びに来たついでに、Steam のフレンド申請も待ってるわ。:-)♪
