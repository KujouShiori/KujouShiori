```asm
;;; ──────────────────────────────────────────────
;;;   世は濁れど、われは清し
;;;     機種 : PC-9801          OS : MS-DOS 5.0
;;;     組方 : MASM 5.1（以下、要所のみ）
;;; ──────────────────────────────────────────────
;;;   世界は八つの窓、ことごとく濁れり。われは其の
;;;   裏返しなり。重なりを求めれば、果ては零なり。
;;; ──────────────────────────────────────────────
        mov     bl, 0FFh        ; 世界（八つの窓、みな濁れり）
        mov     al, bl
        not     al              ; われ ＝ 世界の裏返し
        and     al, bl          ; 重なり ＝ 零
        add     al, '0'         ; 零に、文字の一を添ふ
        mov     dl, al
        mov     ah, 02h         ; DOS の文字出力
        int     21h
        mov     ax, 4C00h       ; 零のまま退出す
        int     21h
;;; ──────────────────────────────────────────────
;;;   ※ 画面に出づるは「0」の一字のみ。世界とわれ
;;;     の重なり、零なりと申す意味に候。
```

ごきげんよう。九条詩織（くじょう しおり）と申しますわ。ID の KujouShiori は、そのままこの名前の読みでございますの。覚えやすいでしょう？

まず、線を一本引かせてください。この頁に書きますのは、いま手を動かしていることだけでございますの。これから先の支度は支度として、別に置いておきますわ。ここに書いてございますことが、すべてではございません。

私は<ruby>遊戯<rp>（</rp><rt>ゲーム</rt><rp>）</rp></ruby>をたしなむ PC ゲーマーでございまして、名古屋大学を卒業し、ことし京都大学の大学院に入りましたの。文学研究科でございます。卒論は日本古代史、いまは日本近代史——昭和の家計簿と京都の町家を史料にして、民衆史のほうを歩んでおりますわ。神話史もちょっぴりかじっておりますのよ。歴史と<ruby>電子計算機<rp>（</rp><rt>コンピュータ</rt><rp>）</rp></ruby>の二刀流でございます。あら、欲張りだなんて仰らないでくださいまし♪

- 【遊】<ruby>蒸気<rp>（</rp><rt>スチーム</rt><rp>）</rp></ruby>歴の長い、いわば古参のプレーヤーですわ。Steam は [KobayashiNana](https://steamcommunity.com/id/KobayashiNana/) でございますの。御友達申請は大歓迎ですのよ♪
- 【居】名古屋市瑞穂区の家と、京都の寮とを行き来しておりますの。通う先は京都大学——〒606-8501、京都府京都市左京区吉田本町でございますわ。住まいの番地までは申しませんのよ。史料と同じで、要らぬところまで曝すことはいたしませんもの。
- 【秘】この<ruby>書庫<rp>（</rp><rt>リポジトリ</rt><rp>）</rp></ruby>には、もうひとつファイルを紛れ込ませておりますの。見つけられるかしら？　うふふ、楽しみにしておりますわ。

### 普請中のもの

**Komorebi Launcher** —— 国内のプレーヤーのために、Prism Launcher を元にした Minecraft: Java Edition の<ruby>起動器<rp>（</rp><rt>ランチャー</rt><rp>）</rp></ruby>を組んでおりますの。ダウンロードミラー、Java の自動設定、OptiFine の導入を備え、いまは土台を据えて細部を普請中でございますわ。Microsoft ログイン用の AppID も、2026 年 11 月 6 日に Mojang の審査を通りましたのよ。

- [KomorebiLauncher/KomorebiLauncher](https://github.com/KomorebiLauncher/KomorebiLauncher) · 案内の頁は [komorebilauncher.github.io](https://komorebilauncher.github.io/) にございますわ。
- 軽量版は [KomorebiLauncher/KomorebiLauncherLite](https://github.com/KomorebiLauncher/KomorebiLauncherLite) にございますの。荷物を減らした旅支度で、身軽なぶん歩くのが速うございますわ。

**Token 計島（token-meter）** —— C#/.NET 製、WinIsland / WinLand 用のプラグインでございますの。手元のログと各社クラウドの利用量 API から、token の消費量・推定費用・残高を島に常駐させて表示いたします。出典は混ぜず、API キーも置かない「足さない」の作りで、[luolangaga/WinLandPlugin](https://github.com/luolangaga/WinLandPlugin) のマーケットへお納めしておりますわ。

### 書庫の<ruby>型録<rp>（</rp><rt>カタログ</rt><rp>）</rp></ruby>

| 書庫 | なにか |
| --- | --- |
| [KujouShiori.github.io](https://github.com/KujouShiori/KujouShiori.github.io) | HTML —— Hexo で組んだ私のブログですわ。日本古代史と神話の文章、それにリソース解析の記録を置いておりますの |
| [YatagarasuMC.github.io](https://github.com/YatagarasuMC/YatagarasuMC.github.io) | HTML —— Minecraft の MOD パックと遊び方を集めて残しておくサイトですの。自分で組んで GitHub Pages に置いておりますわ |
| [BurstWitchCodex.github.io](https://github.com/BurstWitchCodex/BurstWitchCodex.github.io) | JavaScript —— サービスを終えたスマホゲーム『爆裂魔女』の非公式 Wiki。無くなるはずだった資料を、手元から一つずつ起こしておりますのよ |
| [The-Elder-Scrolls-5-Skyrim-All-books](https://github.com/KujouShiori/The-Elder-Scrolls-5-Skyrim-All-books) | スカイリムの作中書物を、一冊残らず抜き出した資料庫ですわ |

もともと遊びたいゲームに中国語がなかったんですもの。それで翻訳を始めた、というのがいちばん本当の動機に近いのでございますわ。Minecraft と galgame のローカライズ、それに消えたら困る資料のアーカイブで、書庫の大半が埋まっておりますの。ゲームのデータベースサイト（MirrorStation、BurstWitchCodex など）も、自分で組んで GitHub Pages に置いてございます♪

もうひとつの軸はバイナリでございます。中国語にしたければ、リソースの形式を読むしかございませんもの。スマホのゲームの Lua をこっそり読み出せたときの喜びったら！　まあ、はしゃぐのは全ファイルで往復確認を済ませてからにいたしましたけれど。中身は、まだ内緒ですの。

他の方の書庫へ直接お納めしたのは、[icey9527/Verviewer](https://github.com/icey9527/Verviewer) の PSD プレビューと汎用位置決めのあたりでございますわ。<ruby>起動器<rp>（</rp><rt>ランチャー</rt><rp>）</rp></ruby>でも MOD でもデスクトップの道具でも、壊れているものを見るとつい報告してしまう性分ですの♪

### 私の道具箱

<p align="center">
  <img alt="C#/.NET" src="https://img.shields.io/badge/C%23%2F.NET-512BD4?style=for-the-badge&logo=csharp&logoColor=white" />
  <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img alt="C++" src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
  <img alt="Assembly" src="https://img.shields.io/badge/Assembly-6E4C13?style=for-the-badge&logo=assemblyscript&logoColor=white" />
  <img alt="Windows 11" src="https://img.shields.io/badge/Windows%2011-0078D5?style=for-the-badge&logo=windows11&logoColor=white" />
  <img alt="NeoForge / Fabric / Bukkit" src="https://img.shields.io/badge/NeoForge%2FFabric%2FBukkit-00AF5F?style=for-the-badge&logo=minecraft&logoColor=white" />
  <img alt="UWP / WPF" src="https://img.shields.io/badge/UWP%2FWPF-7F0B7C?style=for-the-badge&logo=windows&logoColor=white" />
  <img alt="VS Code" src="https://img.shields.io/badge/VS%20Code-0078D7?style=for-the-badge&logo=visual-studio-code&logoColor=white" />
  <img alt="Git" src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img alt="コントリビューション" src="https://hub.xerj.org/contributors/KujouShiori/badge.svg" />
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img alt="Windows Terminal" src="https://img.shields.io/badge/Windows%20Terminal-4D4D4D?style=for-the-badge&logo=windows-terminal&logoColor=white" />
  <img alt="PowerShell" src="https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" />
  <img alt="Visual Studio" src="https://img.shields.io/badge/Visual%20Studio-5C2D91?style=for-the-badge&logo=visualstudio&logoColor=white" />
  <img alt="NuGet" src="https://img.shields.io/badge/NuGet-004880?style=for-the-badge&logo=nuget&logoColor=white" />
  <img alt="IntelliJ IDEA" src="https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white" />
  <img alt="Linux" src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
</p>

<br />

<p align="center">
  <img alt="GitHub の統計" height="180em" src="https://github-readme-stats.zohan.tech/api?username=KujouShiori&show_icons=true&theme=tokyonight&hide_border=true&bg_color=00000000" />
  <img alt="よく使う言語" height="180em" src="https://github-readme-stats.zohan.tech/api/top-langs/?username=KujouShiori&layout=compact&theme=tokyonight&hide_border=true&bg_color=00000000&locale=ja" />
  <br />
  <img alt="訪問者数" src="https://komarev.com/ghpvc/?username=KujouShiori&color=0079d5&style=for-the-badge" />
</p>

> 遊びにいらしたついでに、<ruby>蒸気<rp>（</rp><rt>スチーム</rt><rp>）</rp></ruby>の<ruby>御友達<rp>（</rp><rt>フレンド</rt><rp>）</rp></ruby>申請もお待ちしておりますわ。壊れているものを見つけましたら、そっと教えてくださいませ。それでは、ごきげんよう♪

---

**註**　この頁に書きましたのは、いま手元で確かめられることだけでございます。コミットの数や Issue の件数は数えるたびに変わるものですから、ここには書きません。数は Release の頁と、GitHub の数え方にお任せいたしますわ。
