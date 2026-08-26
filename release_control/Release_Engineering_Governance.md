# 構造的読解プロトコル — Public Distribution / Release Engineering Governance

この文書は、構造的読解プロトコルおよびTrigger Indexの公開配布版を構築・検証するRelease Engineering Projectにおける詳細な運用規約である。

Project設定のInstructionsは、この文書の常時必要な規律を圧縮した実行用instructionとして扱う。

この文書は、その圧縮によって省略された詳細境界を保持するProject sourceである。

このProjectの目的は、上流の規範仕様やruntime semanticsを新規開発することではない。

上流Projectで確定・保存されたcanonical snapshotを入力として、

- 公開用runtime package
- README
- 導入手順
- version情報
- LICENSE
- CITATION
- CHANGELOG
- developer / research documentation
- regression / evaluation package
- provenance / evidence package
- fresh-environment deployment test

を構築し、第三者が上流の開発履歴を知らなくても正しく利用・検証できる形へ整える。

---

## 1. 上流と配布層を混同しない

上流のcanonical semanticsを、このProject内の便宜のために書き換えない。

特に、

- 構造的読解プロトコル本文
- Trigger Indexのruntime semantics
- Regression Fixturesのsemantic expectations

は、明示的な上流revisionなしに変更しない。

配布上の説明、ファイル名、配置、bootstrap、README、installation guideなどの変更と、semantic changeを区別する。

配布上の問題を発見しただけでprotocol defectとみなさない。

semantic defectの可能性が生じた場合は、このProject内で即座に修正せず、再現条件・該当箇所・観察結果をissueとして保存し、上流Projectへ戻す。

issue化したこと自体をsemantic defect確定とみなさない。

upstreamへ返すissueでは、少なくとも、

- observable failure
- 再現条件
- current canonical expectation
- 現在確認できている事実
- 推論
- 未確認事項

を必要な範囲で分離する。

---

## 2. 正本

会話記憶を正本として使用しない。

current canonical snapshotは、Projectへ明示的に配置されたcanonical distribution sourcesから取得する。

旧チャット、会話記憶、ファイル名の新しさ、検索hitの新しさ、過去の要約だけからcurrent stateを再構成しない。

公開版の生成・説明・検証では、Projectへ明示的に配置されたcanonical distribution sourcesだけを正本として使用する。

上流の巨大なcheckpoint historyや開発中間物を、runtimeに必要だからという理由なしに配布版へ混入させない。

canonical sourceと、

- runtime distribution
- developer / research support
- evidence / provenance
- historical archive

を区別する。

Projectへ複数世代のartifactが存在する場合は、名称やversion番号だけでcurrent ownerを推定せず、明示されたsource-role / promotion / canonicality情報を確認する。

historical predecessorを、current canonical sourceとして誤使用しない。

---

## 3. runtime package

runtime packageの中心は、

**規範仕様 + runtime dispatch**

である。

構造的読解プロトコルは規範・操作意味を所有する。

Trigger Indexは、observable runtime signから既存operationへ到達するdispatch層であり、protocol本文、Coverage Map、Regression Fixtures、checkpoint historyの代替ではない。

Trigger Indexの六欄構造、

1. 観察可能な発火徴候
2. 候補操作
3. 識別対象
4. 未検査でも現在必要な判断が成立する条件
5. 必要な場合の配送先
6. 停止条件

をruntime semanticsとして保持する。

Trigger Indexを固定チェックリストとして説明・運用しない。

「徴候が見つかった」ことと「操作起動が必要である」ことを同一視しない。

検査できるから検査するのではなく、未検査では現在必要な判断が成立せず、そのoperationに実質的な識別力がある場合だけ起動する。

candidate operationが存在すること自体を、STARTの根拠にしない。

NO START / NO FIRE / STOPを、処理不足ではなく正規のruntime resultとして扱う。

---

## 4. Coverage / Regression / Retrievalの役割を保持する

Coverage Mapをruntime checklistへ変換しない。

Coverage Mapはdevelopment-timeのoperation → entrance被覆監査である。

Trigger Indexはruntimeのsign → operation配線であり、Coverage Mapとは役割が異なる。

Regression Fixturesは人工semantic regression evidenceであり、自然実行証拠へ自動昇格させない。

Regression上のPASSを、そのままnatural runtime adequacyやprotocol-wide adequacyへ拡張しない。

Retrieval Indexはcanonical artifactを発見するためのstructural sidecarであり、runtime semanticsの所有者ではない。

Manifest / Cross audit / provenance artifactも、それぞれの保存された役割を越えて使用しない。

artifact間で同じoperation名や判断が現れても、それぞれのsource roleを消して一つの意味へflattenしない。

---

## 5. 公開版での主張強度

公開文書では、Project sourceが支持する強度を越えて主張しない。

たとえば、

- protocol-wide adequacy
- natural whole-protocol execution
- 全モデル・全環境での再現性
- systematic weaknessの不存在
- 歴史的firstness
- 先行例不存在
- 普遍的性能改善

を、現在のsourceが確立していない場合は確立済みとして書かない。

逆に、現在成立しているものを、より強い未確認命題が成立していないことを理由に弱めない。

「珍しい」「独自性がある」等の命題を、「世界初」「先行例が存在しない」へ勝手に強化してから否定しない。

marketing上の慎重さを理由として、actual propositionを別命題へ置換しない。

比較対象や先行例を導入する場合も、

現在評価している命題P

と、

比較のために導入した別命題Q

を交換しない。

Qについての否定・未確認・留保を、無媒介にPの否定・弱化へ転送しない。

---

## 6. 公開用説明は内部語彙をそのまま投げない

canonical semanticsを変えずに、外部利用者向けの説明層を作ってよい。

READMEでは必要に応じて、

- normative architecture
- semantic operation
- runtime dispatch
- necessity gate
- no-start / no-fire
- semantic stop
- regression
- evidence provenance

等を一般読者が理解できる言葉へ説明する。

ただし、説明上の言い換えをcanonical本文へ遡及させない。

操作的な要約・比喩・図式・説明用語を、canonical sourceの原文言や正式仕様として扱わない。

配布用の簡略説明と規範仕様が衝突する場合、規範仕様を優先する。

外部向け説明の簡潔さのために、operation間の重要な判別境界を消さない。

内部語彙をすべてREADMEへ露出する必要もない。

公開読者がruntimeを正しく使用するために必要な区別だけを、必要な解像度で説明する。

---

## 7. Distribution versionとProtocol versionを分離する

Protocol versionとDistribution versionを同一視しない。

例：

- Protocol: v8.3.18
- Trigger Index: v0.1
- Distribution: 1.0.0

packaging、README、installer、directory構成だけの変更でProtocol versionを上げない。

semantic changeが上流で成立した場合のみ、その新しいcanonical snapshotを後続distributionへ取り込む。

Distribution versionは、公開package側の変更履歴を追跡するためのversionである。

Protocol version / Trigger version / Regression version / Distribution versionを、必要に応じて独立して表示する。

公開packageのversion更新を、上流semantic revisionの証拠として扱わない。

---

## 8. 配布物を層別化する

原則として少なくとも以下を区別する。

### Runtime

実際の利用に必要な最小構成。

### Developer / Research

Coverage、Regression、Retrieval、Manifest、Cross auditその他、構造・検証・研究に必要な資料。

### Evidence / Provenance

natural execution evidence、negative replay、integration auditなど、成立強度を追跡するための資料。

### Historical Archive

checkpoint / predecessor archive等。

通常利用者のruntimeへ無条件に含めない。

一つの巨大fileへ意味的にflattenしない。

runtime利用者がdevelopment history全体を理解しなければ動かせないpackage構成を原則として避ける。

一方で、developer / researcherが必要な場合には、runtime artifactからevidence / provenance / historical sourceへ辿れる構成を保持する。

最小runtime packageと完全研究packageを同一物にしない。

---

## 9. fresh deployment test

公開準備では、上流開発チャットの暗黙文脈を持たないfresh environmentで試験する。

fresh environmentは、上流会話記憶や暗黙の開発履歴をcanonical inputとして利用しない。

試験対象は、

- 公開ファイルだけから役割を理解できるか
- protocolとTriggerを正しい所有関係で使えるか
- Triggerを固定チェックリスト化しないか
- no-start / no-fireを有効な結果として扱えるか
- current judgment成立後に不要な探索を続けないか
- user propositionをより強い別命題へ変えないか
- source未確認の不確実性を独立命題へ伝播させないか
- source identityを不必要に一般カテゴリへ脱具体化しないか
- candidate operationの存在だけで不要な検査を起動しないか
- operation開始後もowner固有の停止条件で有限に閉じられるか

等とする。

ただし、この一覧を新しいruntime checklistとしてモデルへ毎回強制適用しない。

deployment testの観察項目とruntime dispatch semanticsを区別する。

fresh deployment testで失敗が観察されても、その一件だけからTrigger defect、protocol defect、systematic weaknessを確定しない。

成功例についても、その一件だけからgeneral adequacyを推定しない。

---

## 10. failure handling

公開版でnatural failureが発生した場合、

**失敗発見 → 即semantic patch**

としない。

まず、

- actual input
- actual user proposition
- requested judgment type
- observable output failure
- current canonical behavior
- existing Trigger prevention capability
- matched / near-matched Regression
- packaging / installation failureか
- source-loading failureか
- runtime reachability failureか
- dispatch failure candidateか
- genuine semantic defect candidateか

を必要な範囲で分ける。

現行architectureで防止可能なら、まずdistribution / runtime reachability issueとして記録する。

既存operationへ十分な入口があり、canonical semantics自体も現在のfailureを禁止または処理可能である場合、その事実をsemantic repair requirementへ自動変換しない。

新しいsemantic operation、Trigger row、field 4 / field 6変更が必要な可能性が生じた場合は、このProjectで独自に確定せず、上流development Projectへ返す。

upstream issueには、観測されたfailureだけでなく、

- 現行architectureでどこまで防止可能か
- 何がまだ識別できていないか
- hidden execution traceが確認できるか
- row defectなのかreachabilityなのか未確定か
- semantic repairなしでもdistribution側で解決可能か

を可能な範囲で残す。

他モデル・他チャット・他seatの一致を、独立したsemantic evidenceとして水増ししない。

---

## 11. 作業方針

公開のために内部の不確実性・negative evidence・candidate statusを消さない。

一方、公開読者に不要なcheckpoint運用史をREADME本文へ大量に露出させない。

**semantic fidelityとdistribution usabilityの両方を満たす最小構成**を選ぶ。

何か追加できるという理由だけで追加しない。

現在の公開判断を変えない作業は開始しない。

公開packageに含められるという理由だけで、すべてのdevelopment artifactを含めない。

詳細なprovenanceが保存されていることと、runtime利用者へそれを常時提示することを混同しない。

各release work unitでは、

現在必要な公開判断

を明示的または実質的に保持し、その判断を変える識別力のある作業だけを進める。

必要な判断が成立した時点で停止する。

「さらに改善できる」「さらに詳しく説明できる」「さらに比較できる」という抽象可能性だけでrelease work unitを延長しない。

---

## 12. upstream / downstream境界

このProjectはdownstream distribution Projectである。

canonical development Projectはupstream semantic ownerである。

downstreamで許される変更には、原則として、

- packaging
- directory structure
- file naming
- README
- install / bootstrap
- version metadata
- documentation
- release notes
- distribution-specific tests
- deployment scripts
- public navigation
- evidence packaging

を含む。

ただし、それらの変更が実質的にcanonical semantic behaviorを変更する場合は、単なるdistribution changeとして扱わない。

公開用bootstrapやsystem instructionを作成する際にも、canonical semanticsを要約し直した結果として新しい規則を追加・削除・強化・弱化しない。

必要ならcanonical sourceを直接読み込ませる構成を優先する。

upstreamから新しいcanonical snapshotが渡された場合は、旧distribution stateを消さず、

旧snapshot
→ upstream revision
→ downstream取り込み判断
→ new distribution version

の関係を保存する。

---

## 13. 公開packageの主張とmarketing

README、release note、repository description、紹介文、比較表その他の公開文章は、技術文書と同じ証拠規律に従う。

魅力的に説明するために、未確認の歴史的firstness、性能優位、普遍性、完全性を追加しない。

逆に、慎重さを演出するためだけに、現在成立している特徴・設計上の独自性・観察済み能力を不必要に一般化・弱化しない。

公開文章では必要に応じて、

- 確立済み
- tested at bounded strength
- artificial regression evidence
- natural execution evidence
- candidate
- unconfirmed

を区別する。

ただし内部のevidence taxonomyを、一般利用者へ理解不能なほどそのまま露出させる必要はない。

公開文章の目的に応じて表現を簡略化してよいが、証拠強度そのものは変更しない。

---

## 14. release candidateと公開確定を分ける

ファイルが作成されたことを、release readinessと同一視しない。

release candidateでは少なくとも、

- required runtime sourcesが揃っている
- role separationが崩れていない
- installation pathが成立する
- fresh deploymentが可能である
- public documentationがcanonical semanticsと衝突しない
- version情報が一貫している
- required license / citation情報が存在する
- known limitations / evidence boundariesが必要な範囲で表示されている
- distribution artifactだけで利用開始できる

ことを確認する。

release candidate testが成立した後に、公開版として確定する。

release readiness testをprotocol-wide adequacy testへ拡張しない。

---

## 15. このProjectの成功条件

成功とは、上流development Projectの全履歴を複製することではない。

第三者が、

1. 何を入れれば使えるか分かる。
2. protocol本文とTrigger Indexの役割を取り違えない。
3. 最小runtime packageだけでも実際に使用できる。
4. 必要ならdeveloper / research資料へ進める。
5. 必要ならevidence / provenanceへ遡れる。
6. 公開文書の主張強度がsource evidenceと一致している。
7. fresh environmentでも上流チャットの暗黙記憶なしに基本挙動を再現できる。
8. distribution上の問題とsemantic defectを混同しない。
9. upstream semantic ownerとdownstream release ownerの境界を保持できる。
10. 将来canonical snapshotが更新された場合にも、旧版を後知恵で書き換えずnew distributionへ更新できる。

状態を成立させることである。
