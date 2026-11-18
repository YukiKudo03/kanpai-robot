# 人とロボットのインタラクション(HRI/HCI)から見た「乾杯ロボット」

> 調査上の注意(レポート執筆者向け)
> - 本調査環境では論文本文の取得(WebFetch)がほぼ全ホストで遮断された(ic.kaist.ac.kr, www.sdu.dk, medium.com, arxiv.org, ar5iv.labs.arxiv.org, www.frontiersin.org, pmc.ncbi.nlm.nih.gov)。そのため「Cited Findings」は**検索結果に現れた抄録・リポジトリ記載・ポスター記載の水準**で確認できた内容に限っている。効果量・検定統計量は、検索結果に明示されたもの以外は記載していない。
> - 検索で裏づけが取れなかったが依頼で名指しされた文献は、各節の「Gaps」に「未検証」として書誌のみ挙げた。最終レポートで数値を引用する場合は原典確認が必要。
> - 「自己報告」か「行動指標」かは可能な範囲で明記した。

## 1. 人–ロボット同期:同期して動くロボットに人はラポール・好意・信頼を感じるか

### Takeaway
ロボットの同期的な動きが印象を良くするという証拠はあるが、多くはビデオ評価・小規模・自己報告であり、「同期そのもの」より「ロボットが動いて応答していること」の効果と分離しきれていない。協働の流暢さ(fluency)研究からは、**先読みして動くこと・人を待たせないこと**が主観的な「息が合っている」感を左右するという、乾杯動作に直接使える知見が得られる。

### Cited Findings
- Lehmann, Saez-Pons, Syrdal & Dautenhahn (2015) "In Good Company? Perception of Movement Synchrony of a Non-Anthropomorphic Robot", PLOS ONE 10(5): e0127747, DOI 10.1371/journal.pone.0127747。表出能力の乏しい Care-O-bot 3 を用いた**オンラインのビデオ調査**(対面実験ではない)。物体を扱う課題中の、人の動作に正に同期した小さな動きは「関与している」と解釈され、ロボットへの評価が好意的になった。— [DOAJ 抄録](https://doaj.org/article/1271ca1b69e74c9e8056fb76ad5fdf0d) / [Herts リポジトリ](https://uhra.herts.ac.uk/id/eprint/4811/)
- 同研究では、**負に同期した(逆方向の)動きでも、静止したロボットより評価が高かった**。著者らは「ロボットの動き一般が知覚に強く影響する」と結論づけている。つまり同期固有の効果は限定的で、「動くこと/応答すること」自体の寄与が大きい。— [DOAJ 抄録](https://doaj.org/article/1271ca1b69e74c9e8056fb76ad5fdf0d)
- Mörtl, Lorenz & Hirche (2014) "Rhythm Patterns Interaction – Synchronization Behavior for Human-Robot Joint Action", PLOS ONE 9(4): e95195, DOI 10.1371/journal.pone.0095195。連続運動と離散イベントが混在する反復的共同作業(ピック&プレース)で、目標指向の同期行動をロボットに合成する設計法を提案し、人と対で評価。主眼は同期の**モデル化・実現**であり、社会的評価の効果量を示す研究ではない(検索で確認できた範囲)。— [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC3994045) / [DOI](https://doi.org/10.1371/journal.pone.0095195)
- Lorenz, Weiss & Hirche "Synchrony and Reciprocity: Key Mechanisms for Social Companion Robots in Therapy and Care", International Journal of Social Robotics, DOI 10.1007/s12369-015-0325-8。同期と互恵性を人間の相互作用の二つの鍵メカニズムと位置づけ、高齢者向けコンパニオンロボットを概観し、これらを組み込む将来の方向を論じる**概念・サーベイ論文**(実験的効果量は提示していない)。刊行年は 2015 オンライン/2016 巻号の可能性があり要確認。— [DOI](https://dx.doi.org/10.1007/s12369-015-0325-8)
- Hoffman & Breazeal (2007, HRI '07):人の行動を**先読み(anticipatory)して動くエージェント**と、反応的に動くエージェントを比較。先読み条件で課題効率が有意に向上し、人とロボットの同時動作量などの流暢さ指標に有意差があり、参加者はロボットのチームへの貢献・流暢さをより好意的に評価した。ただし**未訓練の参加者+シミュレートされたロボット**での実験で、実機ではない。— [MIT Personal Robots Group プロジェクトページ](https://robots.media.mit.edu/portfolio/fluent-teamwork) / [MIT DSpace(Hoffman 博士論文)](https://dspace.mit.edu/bitstream/1721.1/41705/2/221976393-MIT.pdf)
- Hoffman (2019) "Evaluating Fluency in Human–Robot Collaboration"(IEEE Trans. Human-Machine Systems)は、流暢さの客観指標として**人のアイドル時間(H-IDLE)、ロボットのアイドル時間(R-IDLE)、同時活動(C-ACT)、機能的遅延(F-DEL)**を導入。後続研究の要約によれば、主観的流暢さは人のアイドル時間と機能的遅延に左右され、ロボットのアイドル時間と同時活動は有意に効かないとされた。ただしこれらの指標は**シミュレート環境の観察者評価**でしか検証されていなかったと後続研究が指摘している。— [後続研究(NSF PAR)](https://par.nsf.gov//servlets/purl/10404887)
- ロボットとのドラミング(Kose-Bagci, Dautenhahn & Nehaniv ほか、University of Hertfordshire):成人との創発的ターンテイキング実験で、**より多くのやりとりを許し「自然な」ターンテイキングを生むモデルが参加者に好まれた**。KASPAR と子ども(22名、別報告で18名)のドラミング模倣ゲームでは、ロボットの応答に短い遅延を入れると子どもの叩くフレーズと休止が長くなったが、**個人差が大きい**と報告されている。— [Herts 研究ポータル](https://researchprofiles.herts.ac.uk/en/publications/drumming-with-a-humanoid-robot-lessons-learnt-from-designing-and-/) / [RobotCub 成果報告 D5.5](https://www.robotcub.org/index.php/robotcub/content/download/1059/3732/file/RC_UNIHER_KD_Deliverable_D5.5.pdf) / [Kose-Bagci et al. 2008](https://www.robotcub.org/misc/papers/08_Kosebagci_Dautehhahn_Nehaniv_A.pdf)

### Inferences
- 乾杯は「一回きりの離散イベントへ二者が同時に到達する」動作であり、Mörtl らの「連続+離散の混合タスクの同期」に分類できる。ロボットは人の腕の振り上げを観測して**到達時刻を合わせにいく(先読み)**設計が望ましく、人が差し出したグラスを空中で待たせる時間(Hoffman の H-IDLE / F-DEL に相当)を最小化することが主観的な「息が合った」感の主要因になると推測される。
- Lehmann らの結果は「完全な同期でなくても、応答して動くだけで静止より良い」ことを示唆する。乾杯の瞬間以外(会話中のうなずき、グラスを持ち上げる予備動作)にも小さな応答動作を入れる価値がある。
- ドラミング研究の「個人差が大きい」という知見から、乾杯のテンポ(差し出しの速さ・保持時間)は固定値ではなく相手に適応させるべきと考えられる。

### Gaps
- 人–人研究で報告される「同期→親和性」の効果量(メタ分析レベル)に対応する、**人–ロボット同期の統合的な効果量は今回確認できなかった**。Lehmann et al. 2015 のサンプルサイズ・検定値も本文未取得のため未確認。
- 未検証(検索で内容を確認できず):Michalowski, Sabanovic & Kozima (2007) の Keepon によるリズム同期研究("A dancing robot for rhythmic social interaction", HRI '07)、Shen, Slovak & Jung (2015) のロボットによる運動模倣とラポールの研究("'Shall we fight?' / robot mimicry" 系、HRI '15)。いずれも依頼文で名指しされたが、今回の検索では結果を取得できなかった。
- 同期の効果が**長期・反復利用で維持されるか**を扱った研究は見つからなかった。

## 2. ロボットとの共同行為:共同主体感(joint agency / we-agency)は人工パートナーにも生じるか

### Takeaway
潜在指標(intentional binding)で見るかぎり、相手がコンピュータやロボットだと共同主体感は**弱まるか生じにくい**という結果が複数ある。ただし近年はこの解釈自体(binding が社会性を反映するのか、we-agency という概念が必要か)に異論が出ており、結論は確定していない。

### Cited Findings
- Grynszpan et al. (2019, Consciousness and Cognition, PubMed 31561189):触覚的な共同行為で、**intentional binding は人間パートナーとのときだけ生じ、ロボットパートナーでは生じなかった**。著者らは「人–ロボットの共同行為は intentional binding を妨げる」と結論。— [PubMed](https://www.pubmed.gov/31561189/)
- Obhi & Hall (2011):Ciardo らによる二次的記述によれば、**intentional binding は人–人条件でのみ見られ、コンピュータ相手では見られなかった**(原典は今回未取得)。— [Ciardo et al. "Reduced Sense of Agency in Human-Robot Interaction"(プレプリント転載)](https://typeset.io/pdf/reduced-sense-of-agency-in-human-robot-interaction-moxcnnsm1c.pdf)
- Ciardo, De Tommaso, Beyer & Wykowska "Reduced Sense of Agency in Human-Robot Interaction":Cozmo ロボット(Anki)と、膨らむ風船を止めるためにコスト(減点)を払う課題を単独/共同文脈で実施する設計。題名のとおり、ロボットとの共同文脈で主体感が低下することを報告(結果の詳細数値は今回未確認)。— [同上](https://typeset.io/pdf/reduced-sense-of-agency-in-human-robot-interaction-moxcnnsm1c.pdf)
- 反証的な近年の結果:2026 年の Frontiers in Psychology 論文(触覚ボタン押し課題)は、**パートナー種別による binding 量の主効果を個人内で認めず**、人–人ペア内では明示的主体感が強い人ほど binding も強いことを報告。著者らは intentional binding は意図性や社会的文脈より**感覚運動的な予測可能性**を主に反映すると結論している。— [Frontiers in Psychology 2026](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2026.1768740/full)
- Le Besnerais, Moore, Berberian & Grynszpan (2024, Frontiers in Psychology, perspective):共同行為における主体感について、**we-agency 概念を放棄してより節約的な枠組みに置き換えるべき**と論じる批判的レビュー。— [Frontiers in Psychology 2024](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2024.1331084/full)

### Inferences
- 「ロボットと一緒に乾杯した」という共同主体感は、自動的には生じない前提で設計すべきである。2026 年の結果が示すように binding が予測可能性に依存するなら、**ロボットの動きが予測しやすく、自分の動作に随伴して結果(クリン、という音)が確実に返ること**が共同感の下支えになると推測できる。
- 人が相手を「意図をもつ主体」とみなす度合い(intentional stance)が効く可能性があるため、乾杯の前に会話 AI が明示的に意図を表明する(「乾杯しましょう」)ことは、単なる演出以上の意味を持ちうる。ただしこれは推論であり直接の実証は未確認。

### Gaps
- 未検証:Sahaï et al. (2019) "Action co-representation and the sense of agency during a joint Simon task: comparing human and machine co-agents"(Consciousness and Cognition)— 依頼文で名指しされたが今回の検索では内容を確認できなかった。
- **物理的な接触を伴う一回性の社会的儀礼(乾杯・握手)における共同主体感**を測定した研究は見つからなかった。既存研究は実験室的なボタン押し・Simon 課題が中心。
- 相手が「LLM の代理として動くロボット」である場合に、主体が AI なのかロボットなのかという帰属の問題を扱った研究は見つからなかった。

## 3. ロボットとの身体接触儀礼:握手・ハグ・タッチ

### Takeaway
握手研究の総括は「相互作用の各フェーズに何らかの同期が存在する」ことであり、視線・声・表情が握手の印象を変える。ハグ研究は「柔らかく、温かく、相手に合わせて締め、相手が離れたい瞬間に即座に離す」ことが好まれると示し、ロボットからの抱き返しは自己開示や寄付(向社会行動)を増やした。一方、ロボットからのタッチの効果は再現が安定しない。

### Cited Findings
- Prasad, Stock-Homburg & Peters (2022) "Human-Robot Handshaking: A Review", International Journal of Social Robotics 14(1): 277–293(オープンアクセス、CC BY 4.0)。主要な結論として、**握手の各フェーズで何らかの形の同期が存在する**こと、**視線・声・表情がロボット握手の知覚に影響する**こと、性格や気分が握手の仕方に関連することを挙げる。— [TU Darmstadt TUprints](https://tuprints.ulb.tu-darmstadt.de/23499) / [DeepAI 抄録](https://deepai.org/publication/human-robot-handshaking-a-review)
- Block & Kuchenbecker (2018/2019) "Softness, Warmth, and Responsiveness Improve Robot Hugs", International Journal of Social Robotics。**参加者 30 名が 12 種のハグ**を体験・評価(圧力と持続時間を低・中・高で操作)。**柔らかく温かいハグが硬く冷たいハグより有意に好まれ**、利用者は「身体を締めてくれて、**自分が終えたいときに即座に離してくれる**」ハグを好んだ。— [MPI-IS 論文ページ](https://is.mpg.de/publications/block18-ijsr-improve) / [ETH Research Collection](https://research-collection.ethz.ch/handle/20.500.11850/306705?show=full)
- HuggieBot 2.0(Block et al. 2021):視覚的なハグ開始検出、触覚による体格への合わせ込み、触覚による解放検出(腕のトルクセンサで離れたい意思を検出)の 3 要因を検証し、**触覚的反応性を加えるとハグロボットの知覚が明確に改善**した。— [arXiv 2101.07679](https://arxiv.org/pdf/2101.07679v1.pdf) / [MPI-IS プロジェクトページ](https://is.mpg.de/hi/projects/huggiebot-how-should-robots-hug)
- Shiomi et al. (2017, RO-MAN):クマ型ロボット。**ロボットに抱き返された参加者は、自分がロボットを抱くだけの参加者より多く寄付した**(N=38、行動指標)。— [ATR 著者版 PDF](https://irc.atr.jp/~m-shiomi/page/PDF/2017_Ro-MAN_Hug_Submit.pdf)
- Shiomi et al. (2017, ICSR):**ロボットに抱かれた参加者は、抱かれなかった参加者より有意に多く自己開示した**(N=32、行動指標)。— [Springer](https://rd.springer.com/chapter/10.1007/978-3-319-70022-9_32)
- Shiomi, Nakata, Kanbara & Hagita (2020) "Robot Reciprocation of Hugs Increases Both Interacting Times and Self-disclosures", International Journal of Social Robotics, DOI 10.1007/s12369-020-00644-x:**抱き返しにより相互作用時間が延び、自己開示が増えた**(N=48)。— [Springer](https://link.springer.com/10.1007/s12369-020-00644-x)
- Willemse & van Erp (2019) "Social Touch in Human–Robot Interaction: Robot-Initiated Touches can Induce Positive Responses without Extensive Prior Bonding", International Journal of Social Robotics 11: 285–304, DOI 10.1007/s12369-018-0500-9:ストレス状況下で、ロボットからのタッチが人のタッチに類する有益な反応を生むか、事前の絆が必要かを検討。題名のとおり、**事前の十分な絆づくりなしでも肯定的反応が生じうる**と報告。— [TNO 公開版](https://publications.tno.nl/publication/34634046/hFFm2D/willemse-2019-social.pdf)
- ただし同グループの先行研究 Willemse, Toet & van Erp (2017, Frontiers in ICT)では、怖い映画の視聴中にロボットがなだめる言葉+肩へのタッチを行う条件で、**仮説はいずれも支持されなかった**(ヌル結果)。— [Frontiers in ICT 2017](https://www.frontiersin.org/journals/ict/articles/10.3389/fict.2017.00012/full)

### Inferences
- 乾杯は握手・ハグと違い**物(グラス)を介した間接的接触**で、接触時間は一瞬、力も小さい。握手研究で問題になる握力・剛性のチューニングよりも、「接触前の接近フェーズの同期」と「接触の瞬間の柔らかさ(コンプライアンス)」が中心課題になると推測される。HuggieBot の教訓(相手に合わせる・相手のタイミングで離す)は「人が当ててきた強さ・位置に受動的に合わせ、押し返さない」設計に翻訳できる。
- Shiomi らの知見(ロボットの「返す」行為が自己開示・向社会行動を増やす)は、**互恵的な応答があること**の価値を示す。乾杯でも「人が差し出したら必ず応じる」随伴性が、単にロボットが一方的にグラスを突き出すより重要である可能性が高い。
- 視線・声・表情が握手の知覚を変えるという Prasad らの総括から、乾杯も動作単体ではなく「乾杯!」の発声と視線のタイミングをセットで設計すべき。

### Gaps
- Prasad et al. のレビュー本文(握手の周波数・持続時間・把持力の具体値、握手チューリングテストの結果)は取得できず、**具体的な数値パラメータは未確認**。
- **ロボットとのハイタッチ(high-five)・フィストバンプの社会的効果を扱った査読研究は、今回の検索では確認できなかった**。
- 「不気味さ」を生む具体的な力・遅延の閾値を示す研究は確認できなかった。

## 4. 物体の受け渡し(ハンドオーバー):乾杯に最も近い動作アナログ

### Takeaway
受け渡し研究は、(1) 受け渡しの意図は手が動き出すずっと前に成立している、(2) 受け渡し位置を見る「共同注意」の視線で人のリーチが有意に早まる、(3) 人らしい軌道が好まれ効率も上がる、(4) 「読みやすい(legible)」動きは予測しやすい動きとは別物で、協働の流暢さ・信頼・快適さを上げる、ということを示している。

### Cited Findings
- Strabala et al. (2013) "Toward Seamless Human-Robot Handovers", Journal of Human-Robot Interaction 2(1): 112–132。人–人の観察研究と人–ロボット実験にもとづき、受け渡しの**物理的側面と社会認知的側面を分けた協調構造**を提案。最も意外な観察として、**受け渡しの意図は手が動き始めるよりかなり前に確立されていることが多い**と報告。— [CMU Robotics Institute](https://www.ri.cmu.edu/publications/towards-seamless-human-robot-handovers/) / [著者版 PDF](https://personalrobotics.cs.washington.edu/publications/strabala2013handoff.pdf)
- Moon et al. (2014) "Meet Me Where I'm Gazing: How Shared Attention Gaze Affects Human-Robot Handover Timing", HRI 2014, pp. 334–341。ロボットが**未経験の参加者 102 名**に水のボトルを手渡し、視線を 3 条件(視線なし/受け渡し位置を見る共同注意視線/共同注意+ターンテイキング視線)で操作。**共同注意の視線手がかりがあると、参加者は差し出された物体に有意に早く手を伸ばした(行動指標)**。ターンテイキング視線つきの受け渡しを好む傾向も見られたが統計的には「傾向」どまり。— [UBC SPIN Lab PDF](https://www.cs.ubc.ca/labs/spin/sites/default/files/local_pdfs/2014_MeetMeWhereImGazing.pdf)
- Ortenzi et al. (2021) "Object Handovers: A Review for Robotics", IEEE Transactions on Robotics 37(6): 1855–1873, DOI 10.1109/TRO.2021.3075365。受け渡しを**(1) 事前フェーズ(pre-handover)と (2) 物理的受け渡しフェーズ**に分けて整理し、手法間の公正な比較のための最小限の評価指標セットを提案。— [arXiv 2007.12952](https://arxiv.org/abs/2007.12952v2) / [MPI-IS](https://hi.is.mpg.de/publications/ortenzi21-tro-handovers)
- 軌道について:**人らしい受け渡し動作が好まれ(Shibata et al. 1997)、より速く効率的な受け渡しにつながる(Huber et al. 2008)**。躍度最小(minimum-jerk)モデルは直線経路を仮定するが、人の受け渡し動作は**曲線経路**をとることが後に示され、二つの躍度最小軌道を組み合わせる Decoupled Minimum Jerk が提案されている(いずれも下記論文の先行研究整理による)。— ["Comparing Subjective Perceptions of Robot-to-Human Handover Trajectories" arXiv 2211.08733](https://arxiv.org/pdf/2211.08733)
- Dragan, Lee & Srinivasa (2013) "Legibility and Predictability of Robot Motion", HRI '13:**予測可能性(predictability)と可読性(legibility)は本質的に異なり、しばしば相反する**動作特性である。可読な動作=観察者が目標を早く推定できる意図表出的な動作。— [CMU Robotics Institute](https://www.ri.cmu.edu/publications/legibility-and-predictability-of-robot-motion)
- Dragan の博士論文 "Legible Robot Motion Planning" (CMU-RI-TR-15-15, 2015) は、実機での人–ロボット協働課題において、**予測可能性・可読性のある動作が課題成績だけでなく協働の流暢さを高め、信頼や快適さといった主観指標も向上させた**と報告。— [CMU Robotics Institute](https://www.ri.cmu.edu/publications/legible-robot-motion-planning/)

### Inferences
- 乾杯は「物を渡さないハンドオーバー」と捉えられる:事前フェーズ(意図の合図・視線・グラスの持ち上げ)→接近→接触→離脱。Strabala らの知見から、**アームが動き出す前に、発話(「乾杯しましょう」)とグラスの持ち上げで意図を成立させる**ことが、タイミングずれの最大の予防策になる。
- Moon らの結果を応用すれば、ロボット(または顔に相当する部位)が**接触予定位置=相手のグラスを一度見てから相手の目に視線を戻す**ことで、人の差し出しが早まり、会合点が安定すると推測される。
- 軌道は直線の等速移動ではなく、**緩やかに立ち上がり緩やかに減速する(躍度最小的な)曲線軌道**で、最終的な目標位置が早い段階で読み取れる(legible)ように、やや誇張して相手側へ弧を描くのが妥当と考えられる。
- Ortenzi らの提案どおり、評価指標(会合までの時間、人の待ち時間、失敗率、主観的流暢さ)を事前に定めておくと、乾杯動作の反復改善がしやすい。

### Gaps
- 受け渡し研究の知見が「グラス同士を当てる」動作にそのまま転用できるかを検証した研究は見つからなかった(乾杯の運動学そのものを扱う HRI 研究は未確認)。
- arXiv 2211.08733 の主観評価結果(どの軌道モデルが好まれたか)は検索結果に含まれず未確認。
- 依頼文にあった "Effects of Robot Motion on Human-Robot Collaboration"(Dragan et al., HRI 2015)という題名の論文は今回の検索では確認できず、博士論文の記述で代替した(未検証)。

## 5. ロボットの視線・アイコンタクト

### Takeaway
ロボットとの相互注視(mutual gaze)は関与感と人らしさの帰属を高め、その後の視線手がかりの効き方も変える。もっとも重要なのは、**「skål(乾杯)」と発声するロボットに対し、直前に相互注視が成立していたかどうかで、人がグラスを上げ返す率が大きく変わった**という野外実験の結果である。

### Cited Findings
- Fischer et al. (2020) "Gaze-Speech Coordination Influences the Persuasiveness of Human-Robot Dialog in the Wild", International Conference on Social Robotics (ICSR 2020)(dblp キー FischerLNRP20)。公共イベントで水を配るロボットが「skål」と言う状況で、**人が応じるかどうかはロボットが事前に相互注視を確立していたかに依存した**。ロボットは**2 名のウィザード(移動担当と対話担当)による遠隔操作**(自律ではない)。— [dblp](https://dblp1.uni-trier.de/rec/conf/socrob/FischerLNRP20.html) / [SDU 著者校正版 PDF](https://www.sdu.dk/-/media/files/om_sdu/institutter/idk/human-robot+interaction_files/2020publication_fischer+et+al_gaze-speech+coordination.pdf)
- 同研究のポスター記載の統計:相互注視条件では、**グラスを上げる(χ²(1,34)=11.806, p=.001)、「skål」と言い返す(χ²(1,34)=9.722, p=.002)**が有意に多かった。**飲む行動の差は有意に達しなかった(χ²(1,34)=1.108, p=.292)**。棒グラフから読み取れるおおよその応答率は、注視なし:飲む約 44%・上げる約 22%・言う約 28%、注視あり:約 62.5%・約 81%・約 81%(グラフ読み取りのため概数)。いずれも行動指標、分析対象は 35 件前後と小規模。— [SDU ポスター PDF](https://www.sdu.dk/-/media/files/om_sdu/institutter/idk/human-robot+interaction_files/2020activites+nov_poster_fischer+et+al_gaze-speech+coordination.pdf)
- 注意:検索結果の要約には「4 つの公共イベントでの約 200 件の相互作用」「ロボットがユーザーを見ながら skål と言うとほぼ全員が直ちに飲み、よそを見ていると 44.5% のみ」という記述もあり、ポスターの「飲む行動は非有意」という記載と**見かけ上食い違う**(分析単位や条件定義が異なる可能性)。原典確認が必要。— [SDU 著者校正版 PDF](https://www.sdu.dk/-/media/files/om_sdu/institutter/idk/human-robot+interaction_files/2020publication_fischer+et+al_gaze-speech+coordination.pdf)
- Kompatsiari et al. (2017, ICSR):iCub が参加者の目を見る条件と下を向く条件を比較。人は人工エージェントの相互注視に敏感で、**相互注視が成立するとロボットへの関与感が高まり、人らしい特性の帰属が促された**。— [Zenodo 著者版](https://zenodo.org/records/1164864/files/Kompatsiari%20et%20al.%20(2017)%20ICSR.pdf)
- Kompatsiari et al. (2018, Scientific Reports):iCub を用いた視線手がかり課題で、**事前のアイコンタクトの有無が視線手がかり効果を調整した**(アイコンタクトなしでは手がかり効果が弱まる/生じない)。— [LMU 公開版 PDF](https://epub.ub.uni-muenchen.de/68076/1/s41598-018-36136-2-1.pdf)

### Inferences
- 乾杯ロボットの設計上もっとも直接的な根拠は Fischer らの結果である:**「乾杯」の発声は相互注視の成立後に行う**。視線を検出できない場合でも、顔(カメラ・目に相当する部位)を相手に向けてから発声・動作を開始するシーケンスにすべき。
- 人の乾杯作法(目を見てからグラスを合わせる)と、Kompatsiari らの「アイコンタクトが後続の視線手がかりの効きを高める」知見を合わせると、**目を合わせる→グラスへ視線を落とす→接触→再び目を合わせる**という視線シーケンスが合理的と推測される。
- 目を持たない(非人型の)アームだけの装置では相互注視が成立しないため、少なくとも「相手の方を向く」向き直り動作や、会話 AI 側の画面上の視線表現で代替する必要があると考えられる。

### Gaps
- 未検証:Admoni & Scassellati (2017) "Social Eye Gaze in Human-Robot Interaction: A Review"(Journal of Human-Robot Interaction 6(1))は、今回の検索ではレビュー本体を取得できず、二次的言及のみ確認。Mutlu らの視線研究も今回は個別に確認していない。
- Fischer et al. 2020 の正確な N、条件定義、著者フルネーム(dblp キーからは Fischer, L…, N…, R…, P… の 5 名)は本文未取得のため未確認。
- 相互注視の**持続時間の最適値**(長すぎる凝視の不快さ)に関する定量的知見は今回確認できなかった。

## 6. 共食ロボット・飲酒コンパニオン・遠隔乾杯:既存システムの総覧

### Takeaway
**ロボットが人とグラスを合わせる(乾杯する)査読研究は存在する**が、確認できたのは KAIST の一系統(CheersBot 2021 → "Enjoy, but Moderately!" CSCW 2023、予備的ユーザ調査 n=20)のみで、乾杯動作そのものの有無を統制した実験は見当たらない。遠隔で一緒に飲む装置は 2006 年の Lover's Cups 以来いくつかあるが、評価はいずれも小規模・定性的である。共食ロボット分野全体も概念提案・パイロット段階が中心である。

### Cited Findings

#### 6-1. 人と乾杯するロボット
- Jung, Jung, Jeong, Kim, Woo, Hong & Lee (2023) "'Enjoy, but Moderately!': Designing a Social Companion Robot for Social Engagement and Behavior Moderation in Solitary Drinking Context", Proc. ACM Hum.-Comput. Interact. 7(CSCW2), DOI 10.1145/3610028(KAIST)。一人飲みの相手をしつつ、飲むペースを調整して節度ある飲酒へ導く社会的コンパニオンロボット。**予備的ユーザ調査(n=20)**で、ロボットは親しみやすい仲間と知覚され、**大半の参加者がロボットの誘導に従い**、社会的インタラクションと行動追跡機能により「賢い友人」と知覚した。— [dblp](https://dblp1.uni-trier.de/rec/journals/pacmhci/JungJJKWHL23.html) / [KAIST 著者版 PDF](https://ic.kaist.ac.kr/files/papers/jung2023enjoy.pdf) / [Crossref](https://api.crossref.org/works/10.1145%2F3610028)
- 同研究の乾杯ロジック(著者らによる ACM CSCW ブログ記事の要約):**ユーザが前回の乾杯から 2.5〜5 分の間にグラスを合わせようとするとロボットは応じ、ユーザから働きかけがないまま前回の乾杯から 5 分を超えるとロボット側から乾杯を持ちかける**。乾杯を応じる時間窓を設けることで飲むペースを律する設計。— [ACM CSCW Medium 記事](https://medium.com/acm-cscw/how-can-a-social-companion-robot-support-enjoyable-but-moderate-solitary-drinking-d0983a508376)
- 同ブログの定性的結果:ロボットの介入は「自分の飲むペースを省みさせることで、速く飲みすぎないよう助けた」。また**「主要な身体的インタラクション(乾杯)が、ユーザとの社会的ラポールを築くことで説得において重要な役割を果たした」**と報告。著者らは乾杯(グラスを合わせること)を「一体感を築くため社会的飲酒で重要」と位置づけている。— [ACM CSCW Medium 記事](https://medium.com/acm-cscw/how-can-a-social-companion-robot-support-enjoyable-but-moderate-solitary-drinking-d0983a508376)
- Kim, Jung et al. (2021) "CheersBot"(HCI Korea 2021、韓国語論文、KAIST):COVID-19 の社会的距離確保下の孤独を和らげるため、飲酒場面の主要なインタラクションである**グラスを合わせる身体的インタラクションと音声インタラクション**を提供する飲酒コンパニオンロボット。論文中のアンケートでは、**回答者の 65% が「乾杯と会話的音声インタラクションの二つがあれば一人飲みがもっと楽しくなる」**と回答(自己報告・意向調査)。— [KAIST リポジトリ](https://dspace.kaist.ac.kr/handle/10203/289347?mode=full) / [著者版 PDF](https://ic.kaist.ac.kr/files/papers/kim2021cheersbot.pdf)
- CheersBot のプロジェクトページ・開発者投稿によれば、ビデオ通話飲みは視覚・聴覚はカバーするが**身体的インタラクションを欠く**という問題意識から出発。TensorFlow Object Detection API で構築し TensorRT で最適化して Jetson Nano 上で実時間動作。機能として乾杯インタラクション、音声認識と応答、飲酒量の追跡、**飲みすぎ時の乾杯拒否**が挙げられている(査読外の情報)。— [NVIDIA Jetson Projects](https://developer.nvidia.com/embedded/community/jetson-projects/cheersbot) / [NVIDIA Developer Forum 投稿](https://forums.developer.nvidia.com/t/cheersbot-if-you-wanna-cheers-with-your-friends-during-self-quarantine-covid-19/140274)
- Fischer et al. (2020):水を配るロボットが「skål」と**発声**し、人がグラスを上げて言い返すかを調べた野外研究(§5 参照)。ロボット側がグラスを物理的に合わせるわけではなく、**言語的な乾杯の呼びかけ**である点に注意。— [dblp](https://dblp1.uni-trier.de/rec/conf/socrob/FischerLNRP20.html)
- 査読外:韓国の発明家による飲酒ロボット「Drinky」(2015–2016 年頃に報道)。一緒に酒を飲み、こぼさずにグラスを合わせられるとされるが、報道記事のみで評価研究はない。— [Hackaday](https://hackaday.com/2016/01/11/drinking-with-your-robot/)

#### 6-2. 遠隔で一緒に飲む・遠隔乾杯の装置
- Chung, Lee & Selker (2006) "Lover's Cups: Drinking Interfaces as New Communication Channels", CHI 2006 Extended Abstracts, pp. 375–380, DOI 10.1145/1125451.1125532(MIT Media Lab)。無線接続された一対のカップで、離れた相手と飲む時間を共有する。報道によれば、片方がグラスを手に取ると相手のグラスの赤色 LED が穏やかに光り、口をつけるとより明るく光る。**二人が同時に飲むとカップが光って共有された親密さを祝う**(SIGGRAPH ポスター版の要約)。— [dblp](https://dblp.org/rec/conf/chi/ChungLS06.html) / [SIGGRAPH History Archives](https://history.siggraph.org/?p=139527) / [Dawn(New Scientist 引用)](https://www.dawn.com/news/182185)
- Lover's Cups の評価:報道によれば「別々の実験室でのテストの後、Lee は無線グラスが飲む体験を共有している感覚を実際に助けると述べた」。**研究デザイン・人数は報道からは不明**で、定量評価は確認できない。— [Network Computing](https://www.networkcomputing.com/careers-and-certifications/toast-across-miles)
- CoasterMe(University of Melbourne):二つのオフィスを WiFi でつなぐコースター型装置。著者らは「距離を越えて飲み物を共有しているかのように感じさせることで、共在感とつながり感を生んだ」と報告(小規模・定性的とみられる。詳細未確認)。— [CORE 公開版](https://core.ac.uk/download/294806989.pdf)
- 特許:日本発とみられる米国特許群「Drinking dramatization glass … and remote toast counter system」(US 10,966,554 / 10,966,555 / 11,019,948 / 11,191,376)。離れた場所の人が一緒に乾杯できるようにする演出グラスと**遠隔乾杯カウンタシステム**を記述。特許であり評価済みプロトタイプの報告ではない(出願人は今回未確認)。— [USPTO 10,966,555](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10966555)
- 査読外の事例:"Toasting over the Internet 2010"(Behance 掲載の制作事例)。ネットワーク越しに顧客と乾杯する装置で、制作者自身が「唯一の欠点は、飲んでいるのが自分たちだけだったこと」と記している。— [Behance](https://www.behance.net/gallery/9916581/Toasting-over-the-Internet-2010)
- 関連(乾杯ではないが飲む所作の拡張):石井ら「飲む行為に付加価値を与えるグラス型ディスプレイ」(エンタテインメントコンピューティング 2022)。底面に小型プロジェクタとカメラを内蔵し、注ぐ・傾ける・眺める所作に応じて映像を投影。— [情報処理学会 EC2022](https://ipsj.ixsq.nii.ac.jp/record/219506/files/IPSJ-EC2022030.pdf)

#### 6-3. 共食ロボット・人工共食コンパニオン
- Mancini, Niewiadomski, Huisman, Bruijnes & Gallagher (2020) "Room for one more? – Introducing Artificial Commensal Companions", CHI EA '20, DOI 10.1145/3334480.3383027。自ら選んで、あるいはやむなく一人で食べる人に、食事中の同伴を提供するロボット/仮想エージェント(Artificial Commensal Companion)の最初の設計と計算モデルを提示。**共食の利益を再現しうる**と主張するが、これは設計提案であり効果の実証ではない。— [TU Delft](https://research.tudelft.nl/en/publications/room-for-one-more-introducing-artificial-commensal-companions) / [著者版 PDF](https://radoslawniewiadomski.github.io/papers/CHI20_mancinietal.pdf)
- Niewiadomski, Bruijnes, Huisman, Gallagher & Mancini (2022) "Social robots as eating companions", Frontiers in Computer Science, DOI 10.3389/fcomp.2022.909844。MyKeepon と Kinect を組み合わせ、人が食べ物を取る・飲食する動作を追跡して事前定義の非言語行動を返すシステムを開発。**参加者 10 名のパイロット**で、ロボットの有無でチョコレートを試食させ、食べ物の選択とロボットの存在へのフィードバックを分析(小規模、参加者には食体験の研究と説明)。— [Frontiers](https://public-pages-files-2025.frontiersin.org/journals/computer-science/articles/10.3389/fcomp.2022.909844/text) / [TU Delft](https://research.tudelft.nl/en/publications/social-robots-as-eating-companions)
- Khot, Arza, Kurra & Wang (2019) "FoBo: Towards Designing a Robotic Companion for Solo Dining", CHI EA '19(Late-Breaking Work)。人の共食者のように振る舞う**スペキュラティブ・デザイン**のプロトタイプ。電池をつまんで腹に入れ、げっぷをし、音を立て、電池の質や鮮度についてコメントすることで「食べる」。目的は社会的活動に一緒に参加して食事者に同伴感を与えること。評価実験の結果は確認できず。— [dblp](https://dblp.uni-trier.de/rec/conf/chi/KhotAKW19.html) / [Niewiadomski et al. 2019 レビュー(Frontiers in Robotics and AI)](https://frontiersin.org/article/10.3389/frobt.2019.00119/full)
- Niewiadomski, Ceccaldi, Huisman, Volpe & Mancini (2019) "Computational Commensality: From Theories to Computational Models for Social Food Preparation and Consumption in HCI", Frontiers in Robotics and AI 6:119, DOI 10.3389/frobt.2019.00119。食の準備・消費にかかわる社会的側面を扱う計算モデル・技術を「Computational Commensality」として整理したレビュー。— [Frontiers](https://frontiersin.org/article/10.3389/frobt.2019.00119/full)
- 日本語文献(徳島大学『人間科学研究』2023 年):大学生・大学院生 **33 名**を、親しい人と食べる群/ロボットと食べる群/一人で食べる群に分け、10 分間の食事前後に孤独感とネガティブ気分を質問紙で測定(参加者間、1 群約 11 名と小規模、自己報告)。**ロボットとの食事は、親しい人との食事と同程度に食事中の孤独感を低減**した。一方、**ネガティブ気分については一人で食べる場合と比べ有意な変化がなかった**。— [CiNii Research](https://cir.nii.ac.jp/crid/1050298588047519616/)
- Fong, Soufargi, Mancini & Niewiadomski (2025) "Designing Interactions for Artificial Commensal Companions"(DIS 2025 Companion)としてこの系統の研究は継続している。— [UniGe IRIS](https://unige.iris.cineca.it/retrieve/cddec0fa-73dd-40a2-a7d0-49a955090b20/3715668.3736351%20DIS.pdf)

#### 6-4. 遠隔共食(ビデオ越しの食事)
- 鎌田ら(ヒューマンインタフェース学会論文誌 28(1), 2026、筑波大学 井上智雄研究室系):学生 **10 名**で、一人食/対面共食/遠隔共食の 3 条件について気分(POMS2)、食事動作、視線、発話を比較(行動データは ELAN で注釈)。抄録の範囲では具体的結果は未確認。— [J-STAGE](https://www.jstage.jst.go.jp/article/his/28/1/28_45/_article/-char/ja)
- 筑波大学修士論文(2013 年頃):遠隔共食と対面共食の発話・視線・食事動作を比較。**食事動作そのものには差があるとはいえないが、食事動作の同調には対面と遠隔で差がある**ことを示した。— [筑波大学 図書館情報メディア研究科](https://www.slis.tsukuba.ac.jp/grad/assets/files/pub/2013/s1121755.pdf)
- 筑波大学修士論文(張, 2021):遠隔二者共食で、相手と同じ菓子を食べる/違う菓子を食べる/食べない、を比較(ビデオ観察+質問紙+インタビュー)。食べない条件では相手以外を見る視線が増えたが、会話や食事行動の指標に大きな差は見られなかった。— [筑波大学 抄録 PDF](https://www.slis.tsukuba.ac.jp/grad/assets/files/pub-2/2021/201921659_abstract.pdf)
- VRSJ 2025:研究室での非同期型「じわじわ忘年会」(各自が短い飲酒動画を撮って Slack で共有)。ロボットは使わないが、リモートワークで終業後の飲み会など非公式コミュニケーションが減ったという問題意識を示す。— [日本バーチャルリアリティ学会大会 2025](https://conference.vrsj.org/ac2025/program/doc/2B1-11.pdf)

#### 6-5. バーテンダーロボット・飲み物提供ロボット
- JAMES プロジェクト(Foster ら):社会的に適切に振る舞うロボットバーテンダー。視聴覚センサから客の**関与状態(engagement)を推定**し、実際に注文したい人にだけ応対する。実際のバーでの人の行動観察に基づく手書きルール分類器と教師あり学習分類器を、オフライン交差検証とオンラインユーザ調査で比較(Foster, Gaschler & Giuliani 2017, International Journal of Social Robotics, DOI 10.1007/s12369-017-0414-y)。複数客の場面では、二人目に待つよう伝え、一人目の取引を終えてから応対する。— [Springer](https://link.springer.com/doi/10.1007/s12369-017-0414-y) / [著者版 PDF](https://vmknoll82.in.tum.de/Main/Publications/Foster2017.pdf)
- 同プロジェクトの "Ghost-in-the-Machine" 研究(Loth et al. 2015, Frontiers in Psychology):人がロボットバーテンダーの「中の人」となって注文対応する手法で、バーでの社会的シグナルを抽出。— [Frontiers in Psychology 2015](https://www.frontiersin.org/articles/10.3389/fpsyg.2015.01641/full)
- 日本機械学会ロボティクス・メカトロニクス講演会 2016:飲み物を必要としている人に飲み物を渡すロボットシステムの研究(乾杯は含まない)。— [J-STAGE](https://www.jstage.jst.go.jp/article/jsmermd/2016/0/2016_1A1-14a3/_article/-char/ja)

### Inferences
- 「ロボットが人とグラスを合わせる」システムの学術的先例は KAIST の CheersBot 系統にほぼ限られ、しかも主目的は**節度ある飲酒への行動変容**であって、乾杯が絆に与える効果の検証ではない。**「会話 AI の代理として乾杯するロボット」は新規性の高い領域**であり、乾杯の有無・タイミング・視線を統制した比較実験はそれ自体が研究貢献になりうる。
- KAIST の「2.5〜5 分の応答窓」「5 分無反応でロボットから誘う」は、乾杯の**頻度・主導権**設計の具体的な出発点として使える(ただし根拠は節酒ペース設計であり、最適値として検証されたものではない)。
- Behance 事例の「飲んでいるのは自分たちだけ」という指摘と、FoBo が電池を「食べる」設計は、**相手が実際には飲食しないことの非対称性**が共食・共飲体験の根本課題であることを示す。乾杯の後にロボット/AI 側が「飲む」ことをどう表現するか(しないか)は設計上の明示的な判断事項となる。
- 徳島大学の結果(孤独感は下がるが気分は変わらない)は、ロボット同伴の効果が**孤独感の低減に限定され、気分の改善までは及ばない可能性**を示唆する。期待値の設定に注意が必要。
- 遠隔共食研究の「動作の同調が対面と遠隔で異なる」という知見は、物理的に同じ場にある装置(ロボット)が同調の場を取り戻す、という設計根拠として使える(推論)。

### Gaps
- **日本語圏の「遠隔乾杯」「エア乾杯」デバイスの査読研究は、今回の検索(J-STAGE・情報処理学会・VRSJ 系を含む日本語クエリ)では見つからなかった**。企業による遠隔乾杯グラスなどの製品・キャンペーン事例は存在する可能性があるが、今回は確認できていない(特許の出願人も未確認)。
- 未検証/未発見:依頼文にあった「Fujii et al. 2020/2021 の共食ロボット(日本)」「Takahashi et al.」「Wei et al. の CoDine」「KIZUNA」「徳久らの遠隔共食研究」「ビール注ぎロボット」は、今回の検索では該当文献を特定できなかった。CoDine は Wei et al. (2011) "CoDine: an interactive multi-sensory system for remote dining"(UbiComp '11)として知られるが、今回内容を確認できていないため未検証とする。
- ARcall(arXiv 2203.04358、AR グラスでの通話、参加者 14 名の定性調査)が検索に現れたが、乾杯との関連は検索要約からは確証が取れず、未検証。
- KAIST 2023 論文の節酒効果の定量指標(飲酒ペース・量)、ロボットのハードウェア構成(アーム自由度、乾杯検出方法、接触力)は本文未取得のため未確認。CheersBot 2021 の機能セットは情報源間で記述が一致していない。
- **乾杯の有無だけを操作してラポール・信頼を比較した統制実験は、ロボットについては一件も見つからなかった。**

## 7. 身体性:物理的にその場にいるロボットは画面エージェントや音声のみより強い社会的効果を持つか

### Takeaway
物理的に同じ空間にいるロボットは、画面上の同じロボットや仮想キャラクタより説得力が高く好意的に知覚されるというのが総括的な結論であり、鍵は「身体を持つこと」ではなく「その場に物理的に存在すること」である。ただし LLM を載せたロボットでは、冗長な応答や誤りが目立つとかえって好まれないという 2024 年の結果があり、身体性は無条件の利点ではない。

### Cited Findings
- Li (2015) "The benefit of being physically present: A survey of experimental works comparing copresent robots, telepresent robots and virtual agents", International Journal of Human-Computer Studies 77: 23–37, DOI 10.1016/j.ijhcs.2015.01.001。**33 件の実験研究**を対象に効果の方向を質的にレビュー。ロボットは、**ユーザと同じ空間に物理的に存在するとき、画面に映された場合(同じロボットのライブ映像でも仮想キャラクタでも)より説得的で、より肯定的に知覚され**、ユーザの成績も良かった。— [Edinburgh Napier リポジトリ](https://napier-repository.worktribe.com/output/3636900/the-benefit-of-being-physically-present-a-survey-of-experimental-works-comparing-copresent-robots-telepresent-robots-and-virtual-agents)
- 同レビュー:物理ロボットと仮想エージェントを**どちらも画面に映した場合は、人の反応に差がなかった**。結論は「人の社会的ロボットへの反応を特徴づけるのは physical embodiment ではなく **physical presence**」。— [同上](https://napier-repository.worktribe.com/output/3636900/the-benefit-of-being-physically-present-a-survey-of-experimental-works-comparing-copresent-robots-telepresent-robots-and-virtual-agents)
- Bainbridge, Hart, Kim & Scassellati (2011) "The Benefits of Interactions with Physically Present Robots over Video-Displayed Agents", International Journal of Social Robotics 3: 41–52, DOI 10.1007/s12369-010-0082-7。人型ロボットが同室にいる条件とライブ映像の条件で、本を移動する簡単な課題を実施。**挨拶と協力は両条件で差がなかった**が、**物理的に存在する条件では、参加者は変わった指示(信頼を要する指示)に従いやすく、ロボットにより広いパーソナルスペースを与えた(行動指標)**。映像に 3D 情報を付加しても差は埋まらず、質問紙でも物理的に存在するロボットとの相互作用の方が全体に肯定的だった。— [Springer](https://link.springer.com/doi/10.1007/s12369-010-0082-7)
- Deng, Mutlu & Matarić (2019) "Embodiment in Socially Interactive Robots", Foundations and Trends in Robotics 7(4): 251–356。「物理的身体性は社会的相互作用の成績と知覚に測定可能な効果をもつ」という**身体性仮説**の現状を既存研究から分析し、身体性の種類・社会的役割・課題の 3 つの分類体系を提示。多くの社会的ロボットは課題遂行に物理的作用を必要としないため、安価な仮想エージェントに対し**いつ身体が見合うのか**が問いとなる、と整理。— [arXiv 1912.00312](https://arxiv.org/pdf/1912.00312) / [now publishers](https://www.nowpublishers.com/article/Details/ROB-056)
- Kim, Lee & Mutlu (2024) "Understanding Large-Language Model (LLM)-powered Human-Robot Interaction", HRI '24。**LLM 搭載の社会的ロボット**を、テキストエージェント、音声エージェント(ロボットを黒い幕で隠して同じ声を使用)と比較(**参加者 32 名**)。LLM 搭載ロボットは期待を高めるが、**LLM の豊かな社会的能力が冗長な応答、論理・コミュニケーション上の誤り、課題中の不安を生む場合には好まれにくい**。身体をもつエージェントへの選好は、身体性だけでなく**課題文脈**に左右される。— [arXiv 2401.03217](https://arxiv.org/html/2401.03217v1) / [著者版 PDF](https://peopleandrobots.wisc.edu/wp-content/uploads/sites/1469/2025/02/3610977.3634966.pdf)
- 人型社会ロボット(能動的傾聴/受動的傾聴)と音声アシスタントをスピーチ練習のコーチとして比較した 2024 年の研究(Paladyn, Journal of Behavioral Robotics):ロボットは両条件とも**人らしさと好ましさで音声アシスタントより肯定的に知覚**。満足・関与・自然さ・温かさで音声アシスタントを上回ったのは**能動的に傾聴するロボットのみ**で、受動的なロボットと音声アシスタントの間には差がなかった。— [De Gruyter](https://www.degruyterbrill.com/document/doi/10.1515/pjbr-2024-0004/html?lang=en)
- Furhat ロボットと音声のみのシステムを瞑想ガイドで比較した研究(University of Glasgow):**身体をもつ条件で社会的存在感の得点が有意に高かった**(刊行年は未確認)。— [Glasgow Enlighten](https://eprints.gla.ac.uk/386301/2/386301.pdf)

### Inferences
- 乾杯は「物理的にその場にいなければ不可能な行為」であり、Deng らの問い(身体はいつ見合うのか)に対する明快な答えになる。会話 AI が画面や声だけでは決してできないことを、物理的存在が初めて可能にする、という設計根拠が立つ。
- Li と Bainbridge の結果は、乾杯ロボットを**映像越しではなく利用者と同じ卓上に置く**ことの根拠になる。
- ただし Paladyn 2024 と Kim et al. 2024 の結果は、**「身体があるだけ」では不十分で、応答的に振る舞って初めて優位が出る**こと、また LLM の応答が冗長・誤りがちだと身体がむしろ期待との落差を拡大しうることを示す。乾杯前後の発話は短く、動作は応答的にすべきと推測される。
- 身体が「誰の」身体なのか(会話 AI 本人の身体か、AI が操作する道具か)は、既存研究が扱っていない新しい設計変数である。

### Gaps
- **OriHime など分身(アバター)ロボットの社会的存在感に関する実証研究は、今回の検索では確認できなかった。**
- 既存の音声/チャット AI に後付けで物理的な「手」だけを与えた場合(全身のロボットではなく単機能のアーム)の効果を調べた研究は見つからなかった。
- Li (2015) の個別研究の効果量や、Bainbridge et al. (2011) のサンプルサイズは抄録水準の確認にとどまり未確認。

## 8. 失敗と修復:タイミングのずれた乾杯・空振りにどう対処するか

### Takeaway
社会的ロボットの小さな失敗は必ずしも好感度を下げず、むしろ上げることがある(プラットフォール効果)。ただしこれは社会的・軽微な失敗についての知見であり、失敗後の対処の仕方が「また使いたいか」と信頼を左右する。

### Cited Findings
- Mirnig et al. (2017) "To Err Is Robot: How Humans Assess and Act toward an Erroneous Social Robot", Frontiers in Robotics and AI 4:21, DOI 10.3389/frobt.2017.00021。人型ロボット NAO が失敗する条件としない条件を比較。**参加者は失敗するロボットを、完璧に振る舞うロボットより有意に好んだ(自己報告の好ましさ)**。一方、**擬人性と知覚された知性の評定には有意差がなかった**。参加者はロボットの失敗を認識したが、それで拒絶するとは限らなかった。著者らはプラットフォール効果と関連づけている。— [Frontiers](https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2017.00021/epub) / [UWE リポジトリ](https://uwe-repository.worktribe.com/output/886930/to-err-is-robot-how-humans-assess-and-act-toward-an-erroneous-social-robot)
- Honig & Oron-Gilad (2018) "Understanding and Resolving Failures in Human-Robot Interaction: Literature Review and Model Development", Frontiers in Psychology 9:861, DOI 10.3389/fpsyg.2018.00861。**52 件の研究**をレビュー。これまでの研究は**インタラクション上の失敗より技術的失敗に偏っている**と指摘し、失敗の伝達→失敗の知覚と理解→解決、の 3 段階からなる情報処理モデル(RF-HIP)を提案。**ロボットが失敗をどう扱うかが再利用意向に影響し(Lee et al. 2010 を引用)、ユーザの信頼にも影響しうる**。— [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC6013580) / [Frontiers](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2018.00861/full)

### Inferences
- 乾杯の空振りや軽いタイミングずれは、**安全で軽微な社会的失敗**の典型であり、Mirnig らの結果からは致命的とは考えにくい。むしろ「おっと、もう一回」と軽く言って**すぐやり直す**修復動作を用意すれば、愛嬌として機能する可能性がある(人同士の乾杯でも空振りは笑いになる)。
- Honig & Oron-Gilad のモデルに沿えば、(1) 失敗をロボット自身が検出して伝える(接触センサ・音で当たったかを判定)、(2) 利用者に何が起きたか分かるようにする、(3) 再試行する、の 3 段を設計に入れるべき。**失敗に気づかず何事もなかったかのように進む**のが最悪のケースと推測される。
- 一方、グラスを強く当てる・倒す・液体をこぼすといった**物理的実害を伴う失敗**は、Mirnig らの「社会的失敗」の範囲を超えるため、好意的に受け取られる保証はない。安全側(弱い力、コンプライアンス、失敗時は引く)に倒す設計が必要。

### Gaps
- Mirnig et al. (2017) のサンプルサイズは今回確認できなかった(未検証)。
- 未検証:Lee et al. (2010) "Gracefully mitigating breakdowns in robotic services"(HRI '10)は、謝罪・補償・選択肢提示などの修復戦略の効果を扱うとされるが、今回の検索では内容を確認できなかった。
- **反復的な失敗**(毎回ずれる)が好感度に与える影響、および物理的接触を伴う失敗(衝突・こぼす)に対する人の反応を扱った研究は確認できなかった。プラットフォール効果は元の対人研究でも「有能な相手の失敗」に限られるとされるが、ロボットでの境界条件は未確認。

## 9. リスクと批判:欺瞞・過度な愛着・新奇性の減衰・アルコールとの結びつき

### Takeaway
社会的ロボットには、意図の有無にかかわらず「欺瞞」が生じうるという倫理的批判と、感情的愛着の形成への懸念がある。長期利用では新奇性が薄れると関与が落ちることが指摘されている。アルコールに関しては、確認できた唯一の乾杯ロボット研究が「節度ある飲酒への誘導」を設計目的に組み込んでいる点が示唆的である。

### Cited Findings
- Sharkey & Sharkey (2021) "We need to talk about deception in social robotics!", Ethics and Information Technology:社会的ロボティクスには、**意図されているか否かにかかわらず欺瞞が存在しうる**と論じる。— [White Rose リポジトリ](https://eprints.whiterose.ac.uk/180990)
- 高齢者を対象とした縦断研究(Frontiers in Robotics and AI, 2020)は、ロボットの感情表出が**感情的欺瞞**につながりうること(Sharkey & Sharkey 2012 を引用)、ロボットへの**感情的愛着**の形成が別の倫理的懸念であること(Sullins 2012 を引用)を倫理的論点として挙げている。— [Frontiers in Robotics and AI 2020](https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2020.00001/pdf)
- Leite, Martinho & Paiva (2013) "Social Robots for Long-Term Interaction: A Survey", International Journal of Social Robotics 5: 291–308, DOI 10.1007/s12369-013-0178-y:社会的ロボットとの長期的インタラクション研究を概観し、長期研究の知見とロボットの主要特徴を整理。— [Springer](https://link.springer.com/content/pdf/10.1007/s12369-013-0178-y.pdf)
- Leite らの関連論文(2014、共感的ロボットの長期研究)は、**「新奇性効果」が薄れると関与が低下しうる**と述べている。— [Springer](https://springerlink.bibliotecabuap.elogim.com/content/pdf/10.1007/s12369-014-0227-1.pdf)
- アルコールとの関係:Jung et al. (2023, CSCW) は一人飲みの相手ロボットを**節度ある飲酒へ導く**ものとして設計し、乾杯に応じる時間窓によって飲酒ペースを調整した。CheersBot の開発者投稿でも「飲みすぎたら乾杯を拒否する」機能が挙げられている。— [dblp(Jung et al. 2023)](https://dblp1.uni-trier.de/rec/journals/pacmhci/JungJJKWHL23.html) / [NVIDIA Developer Forum](https://forums.developer.nvidia.com/t/cheersbot-if-you-wanna-cheers-with-your-friends-during-self-quarantine-covid-19/140274)
- 期待と現実の落差:Kim, Lee & Mutlu (2024) は、LLM 搭載ロボットが期待を高める一方で誤りや冗長さがあると選好が下がることを示した(§7)。— [arXiv 2401.03217](https://arxiv.org/html/2401.03217v1)

### Inferences
- 乾杯は「一緒に飲む」ことを含意する儀礼だが、ロボット/AI は飲まない。乾杯後に飲むふりをさせる演出は Sharkey らの言う欺瞞の論点に触れうる。**飲めないことを隠さず、乾杯という行為そのものを共有する**という位置づけの方が倫理的に堅い、と考えられる。
- 乾杯ロボットは一人飲みを「楽しくする」方向に働くため、飲酒量・頻度を増やすリスクがある。KAIST の先例にならい、**乾杯の頻度制限、ノンアルコール飲料(お茶・水)での乾杯を同等に扱うこと、飲酒を促す発話をしないこと**を設計原則に含めるべきと推測される。Fischer らの実験が水で行われたことも、乾杯の儀礼がアルコールを必須としないことの傍証となる。
- 新奇性の減衰を考えると、乾杯動作そのものの物珍しさに依存する設計は長続きしない。乾杯を**会話の節目(一日の終わり、達成の祝い)に結びつけ、文脈に意味をもたせる**方が長期的価値につながると推測される。
- 孤独な利用者がロボットとの乾杯に依存し、人との交流を代替してしまう懸念に対しては、遠隔の人と一緒に乾杯する用途(CheersBot の当初の発想)を併せ持たせることが緩和策になりうる。

### Gaps
- **ロボットや AI コンパニオンが飲酒行動(量・頻度)に与える影響を測った統制研究は、KAIST の予備調査(n=20、定量結果未確認)以外に見つからなかった。**アルコールと社会的ロボットの結びつきを正面から論じた倫理論文も確認できなかった。
- 不気味の谷(uncanny valley)に関する文献は、今回は個別に調査していない。非人型のアーム型装置にどこまで当てはまるかは不明。
- Leite et al. (2013) サーベイ本体が新奇性効果をどう扱っているかは本文未取得のため未確認(新奇性の記述は 2014 年の関連論文で確認)。Sharkey & Sharkey (2012) の原典内容は二次引用による確認のみ。
- 乾杯ロボットの**長期利用**(数週間以上)に関する研究は存在しない(確認できた範囲)。
