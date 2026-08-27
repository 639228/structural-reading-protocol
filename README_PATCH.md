# README.md patch for Distribution 1.0.4

Apply exactly these downstream documentation changes to the current published `1.0.3` README.

1. Change the top distribution identity:

```diff
-**配布版:** `1.0.3`
+**配布版:** `1.0.4`
```

2. In `## ライセンスと引用`, replace:

```text
ライセンス範囲と表示条件は `LICENSE.md`、推奨引用形式は `CITATION.md` を参照してください。
```

with:

```text
ライセンス本文は `LICENSE.md`、適用範囲・帰属表示に関する補足は `NOTICE.md`、推奨引用形式は `CITATION.md` を参照してください。
```

3. In `## バージョン`, change only:

```diff
-- Distribution: `1.0.3`
+- Distribution: `1.0.4`
```

No runtime, bootstrap, Trigger, Protocol, Regression, or evidence-strength wording is changed.
