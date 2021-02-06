２０２０卒論用レポジトリ

# 2020gsc_shunsuke-yoda

2021 ゼミ論

日本全国のラーメン二郎店舗位置情報オープン化とメタデータオープン化の実践
Contributing for Ramen Jiro shop geolocation dataset as open data in Japan.
２０２１年１月２５日
青山学院大学 地球社会共生学部 地球社会共生学科
依田 峻輔/shunsuke yoda
学生番号 1A117179
指導教員 古橋 大地 教授
© Furuhashi Laboratory/Shunsuke Yoda, CC BY 4.0

# 概要

本研究は、2021年現在営業中のラーメン二郎全41店舗の地理空間情報を、OpenStreetMap（以下OSM）データベース内に登録し、誰もが自由にラーメン二郎店舗データにアクセスし、再利用することが可能な状況を構築することを目指すものである。
中国由来の麺文化でありながらも、日本に伝播する過程の中で独自の進化を遂げ、2021年現在、代表的な日本の文化の象徴として、グローバルに広く親しまれているラーメン。その中でも「ラーメン二郎」というラーメンブランドは、こってりとした味付けと、満腹感を重視したコストパフォーマスの良いラーメンを提供し、「ジロリアン」という熱狂的なファンや、「二郎系」と呼ばれる新しいジャンルまでもを生み出した。このラーメン二郎の位置情報に関しては2019年度同ゼミ卒業生である渡辺結南氏によって日本全国網羅され、二次利用可能なオープンデータ化がされた。
そこで本研究において、すべての店舗を現地調査することにより、誰もが自由にラーメン二郎店舗データにアクセスし、再利用することが可能な状況を構築することを試みた。
その結果、OSMデータベース内にラーメン二郎全41店舗の情報を入力、データの統一をした。その際に既存データの見直しも行い、そのタギングルールを統一させた。
# 全体構成(IMRAD形式)
## Introduction:
本来、中国由来の麺文化である「拉麺（らーめん）」は、日本に伝播する過程の中で独自の進化を遂げ、日本の「ラーメン」という食文化を確立し、2021年現在、代表的な日本の文化の象徴として、広く親しまれている。その中で、1968年に創業した東京都港区三田を拠点としている「ラーメン二郎」というラーメンブランドが存在する。こってりとした味付けと、満腹感を重視したコストパフォーマスの良いラーメンを提供する店舗だ。ラーメン二郎は、三田での創業以降、独特の味つけと提供方法で、日本のラーメンの中で、「二郎系」という１つのジャンルを確立した。2021年現在、ラーメン二郎は日本に41店舗存在し、暖簾分けシステムというシステムの中で、日本各地に店舗を広げている。これらの二郎系ラーメン愛好家は「ジロリアン」と呼ばれ、各地の二郎系店舗を食べ歩き、その情報共有ウェブサイトも数多く存在する。
一方で、2019年の段階ではラーメン店舗マップとしてラーメン二郎の位置情報が日本全国網羅され、二次利用可能なオープンデータ化がされている例は見当たらないことから、ラーメン二郎のアプリやマップを作る上で、そのデータをオープンに公開・共有することは車輪の再発明と呼ばれる現地調査重複の無駄を省き、ジロリアンらの活動を支える基礎資料となる。併せて、それらのデータを共有するために必要なプラットフォームには何を選択すべきか検討を行い、OSMデータベース内への格納が現実的であると判断し、現地調査によって得られた日本全国のラーメン二郎店舗情報をマッピングを渡辺氏が行ったことで、OSMのオープンな地理空間情報プラットフォームを用いて、日本全国のラーメン二郎店舗データ、およびそのメタデータを整理、網羅することによって、誰もが自由にラーメン二郎店舗データにアクセスし、再利用することが可能な状況が構築構築された。
以上のことから、本研究ではOSMでのラーメン二郎の既存店舗情報の整理及び、持続可能性について試作して行く。
## Methods:
OSM上のラーメン二郎の整理されていなかった店舗情報を整理した。
全41店舗（2021年1月時点）の中で先行研究では実装されて居なかったタグ「wikidata」「wikipedia」の実装
wikidataをOSMと連携させることによってOSMに無いデータを使った検索が可能になることから、OSMというツールが世の中においてより一般的なものになり社会において活躍の場の拡大が目的とする。
## Results:
現在営業中であるラーメン二郎全41店舗の店舗情報を全て整理し、OSM上に公開した。情報源は現地調査（source=survey）である。
2019年の渡辺氏がマッピングを行った以降の「前橋千代田橋店」「千葉店」「大宮公園駅前店」の情報を渡辺氏のタギングルールに従い更新を行った。
wikidataのタグを追加したことで「ラーメン二郎」自体の名称項目の規格が統一されただけでなくOSM上の「ラーメン二郎」が他のオープンデータと連携されたことで、OSMから多数のwikidataと連携した情報にアクセスすることが可能になった。
## Discussion:
主な論点は次の２点である。
1. ラーメン二郎のwikidata内の言語数が少なくグローバルに対応し入れていない。現在ラーメン二郎のwikidataは「日本語、英語、韓国語」のみであり、圧倒的に他言語での表記が少ない。

2. 現在存在するwikidataは「ラーメン二郎」と大別されているが、ラーメン二郎は各店舗ごとに全く別物と言っていいほど、運営方針や味に特徴があることから「ラーメン二郎」自体のwikidataは一般的な情報にしかすぎないことから「各店舗ごと」のwikidataが今後必要になると考える。

## Conclusion:
本研究を通じて、筆者が現地調査を基に収集したラーメン二郎41店舗分の地理空間情報をOSMデータベース内に登録し、既存データの見直しも行い、渡辺氏のタギングルールに従い更新を行った。また、渡辺氏のリファレンスにのっとり、ラーメン二郎の店舗出店及び閉店などの変化や、二郎系と呼ばれる類似のラーメン店等についての情報をOSM上で編集を行うことができた。
## Acknowledgements/謝辞:
本研究を進めるにあたり青山学院大学地球社会共生学部教授の古橋大地（@mapconcierge）氏をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

プレゼン
https://docs.google.com/presentation/d/1iqkmNKbN3XjBRiMiWt-4SuJn2JCaIvxopRj32U5ZhvA/edit#slide=id.gb881f3b244_0_113

参考文献リスト
https://docs.google.com/spreadsheets/d/1HY2Xs53Ov_mdDkS149Kwn3oSsAPGMFlYUOMafZUhiGc/edit?usp=sharing

渡辺氏卒論
https://docs.google.com/document/d/1ZHgPC9dctxyxneaca7BJE46A55MHmba_xuZc7RGYYDE/edit#

進捗プロジェクト
https://github.com/furuhashilab/sotsuron2020/projects/2
