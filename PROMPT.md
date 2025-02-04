template of pronpt {
  f:I→O|{}
  I|{}
  O|{}
  f|{}
  Structure(tree)|{}
  Architecture (marmaid)|{}
  Design(CSS)|{}
}

now creating prompt{
  f:I→O|{Githubを用いたオープンソースの教科書を作成する} 
  I|{相対性理論、量子力学、素粒子物理、熱力学に立脚した化学の知識}  
  O|{相対性理論、量子力学、素粒子物理、熱力学に立脚した化学の教科書}  
  f|{Notebook (.ipynb) を用いた演習問題や試行実験を盛り込み、Github Pages や Colab/Binder との連携も踏まえて最適な方法を考えてください} 

  Structure(.md;tree)|{
以下のようなディレクトリ構造を想定してください。

~~~markdown
# Repository Structure

Chemistry-Relativity-QM-Book/
├── README.md
├── LICENSE
├── docs/
│   ├── 00_Introduction.md
│   ├── 01_Basics_of_Relativity.md
│   ├── 02_Quantum_Mechanics_Primer.md
│   ├── 03_Particle_Physics_and_Atomic_Structure.md
│   ├── 04_Thermodynamics_Foundations.md
│   ├── 05_Chemical_Bonding_in_Relativistic_Contexts.md
│   ├── 06_Quantum_Chemistry_Basics.md
│   ├── 07_Particle_Interactions_in_Chemical_Reactions.md
│   ├── 08_Relativistic_Effects_in_Heavy_Elements.md
│   ├── 09_Advanced_Thermodynamics_for_Chemistry.md
│   ├── 10_Summary_and_Future_Perspectives.md
│   └── references/
│       ├── reference_list.md
│       └── external_links.md
├── examples/
│   ├── experiment_simulations/
│   │   ├── quantum_sim_1.ipynb
│   │   └── thermo_sim_1.ipynb
│   ├── sample_chapters/
│   │   └── advanced_topic_example.md
│   └── figures/
│       ├── relativity_diagram.png
│       ├── quantum_well_diagram.svg
│       └── ...
├── exercises/
│   ├── ch01_exercises.md
│   ├── ch01_exercises.ipynb
│   ├── ch02_exercises.md
│   ├── ch02_exercises.ipynb
│   ├── ...
│   └── solutions/
│       ├── ch01_solutions.md
│       ├── ch02_solutions.md
│       └── ...
├── translations/
│   ├── en/
│   │   ├── 01_Basics_of_Relativity_en.md
│   │   ├── ...
│   └── ...
└── .github/
    ├── ISSUE_TEMPLATE/
    │   └── chapter_issue_template.md
    └── PULL_REQUEST_TEMPLATE.md
~~~

- `README.md`: リポジトリ概要  
- `LICENSE`: 使用ライセンス（CC-BY や MIT など）  
- `docs/`: 教科書本文と関連資料  
- `examples/`: シミュレーションやサンプルコード  
- `exercises/`: 演習問題（.md / .ipynb 併用）と解答  
- `translations/`: 多言語化用ファイル  
- `.github/`: コミュニティ運営用のテンプレート

}

  Architecture(.marmaid)|{
以下は教科書制作から公開までを俯瞰するMermaidダイアグラムの例です（他の出力とは独立）。

~~~mermaid
flowchart TB
    A[執筆者が各章を作成<br>ローカルでMarkdownや.ipynbを編集] --> B[GitHubへPush/PR]
    B --> C[GitHub ActionsでLint/Build実行]
    C --> D[Peer Review<br>Pull Request]
    D --> E[マージ完了]
    E --> F[CI/CDでHTMLに変換し<br>GitHub Pages等にデプロイ]
    F --> G[読者がWeb上で閲覧し<br>Colab/BinderでNotebook実行]
    G --> A[フィードバックを受け<br>更に改良/追記]
~~~

}

  Design(.CSS)|{
以下は中学生を主な対象に、シリコンバレーの最先端SaaSに慣れた小学生にも「おしゃれ」と感じてもらうためのCSS例です。

~~~css
/* ---------------------
   Basic Reset
---------------------- */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ---------------------
   Body and Typography
---------------------- */
body {
  font-family: 'Noto Sans JP', sans-serif;
  background: #F8FAFD;
  color: #333;
  line-height: 1.6;
}

h1, h2, h3 {
  font-weight: 700;
  color: #444;
  margin-bottom: 0.8em;
}

/* カード風レイアウト */
.card {
  background: #FFF;
  border-radius: 0.75rem;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
  padding: 1.5rem;
  margin: 1rem;
}

h1.title {
  font-size: 2.2rem;
  color: #2C3E50;
}
h2.subtitle {
  font-size: 1.6rem;
  color: #606060;
  margin-bottom: 1rem;
}

/* ---------------------
   Navigation or Header
---------------------- */
header {
  display: flex;
  align-items: center;
  padding: 1rem 2rem;
  background: linear-gradient(135deg, #E8F1FF, #C4E1FF);
}

header .logo {
  font-size: 1.8rem;
  font-weight: bold;
  margin-right: auto;
  color: #0E6BA8;
}

header nav a {
  text-decoration: none;
  color: #0E6BA8;
  font-weight: 600;
  margin: 0 0.5rem;
}

header nav a:hover {
  color: #0A4C7D;
  transition: 0.3s;
}

/* ---------------------
   Buttons
---------------------- */
.button {
  background-color: #88D18A;
  border: none;
  border-radius: 0.5rem;
  padding: 0.7rem 1.2rem;
  color: #fff;
  font-weight: 600;
  cursor: pointer;
}

.button:hover {
  background-color: #73BB76;
  transition: 0.3s;
}

/* ---------------------
   Highlighted Section
---------------------- */
.section-highlight {
  background: linear-gradient(135deg, #FFEAF6, #FFD6EC);
  padding: 2rem;
  border-radius: 1rem;
  margin: 2rem 0;
}

/* ---------------------
   Card Hover Effect
---------------------- */
.card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 10px rgba(0,0,0,0.15);
  transition: 0.2s;
}
~~~

}

}

========================================================
■ Critique & Proposals

1. **段階的難易度調整**  
   - 相対性理論や量子力学を扱うにあたり、中学生が理解しやすい視覚資料やストーリーラインを整備する  
   - 数式の展開を本格的に行う前に、実験事例や歴史的エピソードを交えて興味を維持する  

2. **GitHub活用のメリット・リスク**  
   - `.ipynb` ファイルをBinder/Colab連携で手軽に実行できるようにし、環境構築のハードルを下げる  
   - バージョン管理の混乱を避けるため、`nbstripout` などを導入し、不要なメタ情報をコミットしない運用を検討  

3. **コミュニティ形成**  
   - 中学生でも気軽にIssueやDiscussionに書き込みできる仕組みをつくり、教材の改良を双方向で進める  
   - 英訳や他言語版の展開を促し、国際的な学習資源として機能させる  

以上を踏まえてNotebook演習の導入や静的ホスティング＋インタラクティブ連携が実現できれば、相対論・量子力学・素粒子・熱力学を基盤にした化学の教科書プロジェクトを円滑かつ継続的に運用できると考えられます。
