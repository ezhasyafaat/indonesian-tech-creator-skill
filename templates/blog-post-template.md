# Blog Post Template

## Quick Reference
- Length: 1000-2500 words (sweet spot: 1500 words)
- Structure: Title → Intro → Sections → Conclusion
- SEO: Keywords in title, H2s, first paragraph, meta description
- Visuals: Screenshots, diagrams, code blocks every 300-500 words

---

## Template

```markdown
# [SEO-Optimized Title with Primary Keyword]

![Featured image: description]

[Intro hook: 2-3 sentences that grab attention and state the problem]

[What reader will learn: 1-2 sentences]

## [H2: First Main Section]

[Opening paragraph explaining this section]

### [H3: Subsection if needed]

[Content with code examples, screenshots, or diagrams]

```[language]
// Code example if relevant
```

[Explanation of code/example]

### [H3: Another subsection]

[More content]

## [H2: Second Main Section]

[Opening paragraph]

[Content with visuals]

## [H2: Third Main Section]

[Opening paragraph]

[Content with visuals]

## [H2: Conclusion / Summary]

[Recap main points: 3-5 bullet points]

[Next steps for reader]

[CTA: comment, share, related articles]

---

**Meta Description:** [150-160 characters summarizing the post]

**Tags:** [5-10 relevant tags]

**Related Articles:**
- [Related article 1]
- [Related article 2]
```

---

## Example: Git Tips Blog Post

```markdown
# Git Tips dan Tricks untuk Developer Indonesia: Panduan Lengkap 2025

![Developer using terminal with git commands]

Pernah nggak sih kamu kehilangan perubahan karena salah commit? Atau bingung kenapa commit history berantakan? Kamu nggak sendirian. Banyak developer Indonesia yang masih struggle dengan Git, padahal tool ini bisa bikin hidup kamu jauh lebih gampang.

Di artikel ini, kamu bakal belajar git tips dan tricks yang dipakai senior developer sehari-hari. Dari selective staging sampai interactive rebase, semua bakal kita bahas dengan contoh yang relate sama workflow kamu.

## Kenapa Git Mastery Itu Penting

Sebelum kita masuk ke tips, penting untuk paham kenapa Git itu critical. Git bukan cuma "save code". Git itu:

- **Time machine** untuk code kamu
- **Collaboration tool** yang dipakai semua tim
- **Portfolio** yang dilihat recruiter
- **Safety net** kalau ada bug di production

Developer yang jago Git bakal 3-5x lebih produktif dari yang nggak. Serious.

## Tip 1: Selective Staging dengan `git add -p`

Kebanyakan developer pakai `git add .` atau `git add -A`. Ini mistake.

Kenapa? Karena kamu add SEMUA perubahan, termasuk yang belum selesai, debug code, atau temporary files. Commit kamu jadi kotor.

**Solusi: `git add -p`**

```bash
$ git add -p
```

Ini interactive staging. Git bakal nunjukin setiap perubahan (hunk) dan tanya "mau di-staging nggak?". Kamu bisa pilih:

- `y` — yes, stage this hunk
- `n` — no, skip this hunk
- `s` — split this hunk into smaller ones
- `e` — edit this hunk manually

**Contoh use case:**

Kamu lagi fix bug, tapi nggak sengaja ubah formatting di file lain. Dengan `git add -p`, kamu bisa stage cuma perubahan bug fix, skip formatting changes.

```bash
$ git add -p
diff --git a/src/app.js b/src/app.js
@@ -10,6 +10,8 @@ function calculateTotal(items) {
-  return items.length;
+  const total = items.reduce((sum, item) => sum + item.price, 0);
+  return total;
Stage this hunk [y,n,q,a,d,?]? y
```

Result: Commit kamu bersih, cuma ada bug fix. Formatting changes bisa di-commit terpisah nanti.

## Tip 2: Fix Last Commit dengan `git commit --amend`

Pernah commit terus sadar lupa masukin satu file? Jangan commit ulang!

**Solusi: `git commit --amend`**

```bash
$ git add forgotten-file.js
$ git commit --amend
```

Ini update commit terakhir dengan perubahan baru. Kamu bisa:

- Tambah file yang lupa
- Edit commit message
- Update perubahan kecil

**Warning:** Jangan amend commit yang udah di-push ke shared branch. Ini rewrite history dan bakal bikin conflict buat tim.

**Best practice:** Amend cuma untuk commit lokal yang belum di-push.

## Tip 3: Save Work in Progress dengan `git stash`

Kamu lagi di tengah feature, tiba-tiba ada urgent bug yang harus di-fix. Switch branch sekarang? Nggak bisa, working directory kotor.

**Solusi: `git stash`**

```bash
$ git stash save "working on checkout feature"
```

Ini simpan semua perubahan ke "stack". Working directory jadi clean, kamu bisa switch branch dan fix bug.

Udah selesai fix bug? Balik ke branch tadi dan apply stash:

```bash
$ git checkout checkout-feature
$ git stash pop
```

Perubahan kamu balik, siap dilanjut.

**Pro tip:** Kamu bisa stash multiple times dan pilih mana yang mau di-apply:

```bash
$ git stash list
stash@{0}: WIP on main: working on checkout feature
stash@{1}: WIP on develop: fixing login bug

$ git stash apply stash@{1}
```

## Tip 4: Interactive Rebase untuk Clean History

Commit history kamu kayak gini?

```
fix bug
oops
typo
actually fix
wip
final fix
```

Ini nightmare buat review dan debugging.

**Solusi: `git rebase -i`**

```bash
$ git rebase -i HEAD~5
```

Ini buka interactive rebase untuk 5 commit terakhir. Kamu bisa:

- **Squash** — gabung beberapa commit jadi satu
- **Reword** — edit commit message
- **Reorder** — ubah urutan commit
- **Drop** — hapus commit

**Contoh:**

```
pick abc1234 fix bug
squash def5678 oops
squash ghi9012 typo
reword jkl3456 actually fix
drop mno7890 wip
pick pqr1234 final fix
```

Result: History jadi clean, cuma ada 2 commit yang meaningful.

**Warning:** Sama kayak amend, jangan rebase commit yang udah di-push ke shared branch.

## Tip 5: Cherry-Pick untuk Selective Commits

Kamu punya commit bagus di branch experimental, tapi mau pakai di main tanpa merge semua perubahan.

**Solusi: `git cherry-pick`**

```bash
$ git checkout main
$ git cherry-pick abc1234
```

Ini "copy" commit abc1234 ke branch main. Commit lain di experimental branch nggak ikut.

**Use case:**

- Hotfix dari feature branch ke main
- Share specific commit dengan tim
- Backport fix ke older version

## Kesimpulan

Git mastery itu skill yang high-leverage. Lima tips ini aja bisa bikin kamu 3x lebih produktif:

1. **`git add -p`** — selective staging, commit bersih
2. **`git commit --amend`** — fix last commit tanpa commit ulang
3. **`git stash`** — save work in progress, switch branch dengan aman
4. **`git rebase -i`** — clean commit history
5. **`git cherry-pick`** — selective commits antar branch

Mulai dari satu tips dulu, praktekin sampai jadi habit, baru move ke next. Dalam 2 minggu, Git workflow kamu bakal beda banget.

---

**Meta Description:** Belajar 5 Git tips dan tricks yang dipakai senior developer Indonesia. Dari selective staging sampai interactive rebase, panduan lengkap untuk developer yang mau lebih produktif.

**Tags:** git, tips, tricks, developer indonesia, tutorial, version control, productivity, workflow, commit, staging

**Related Articles:**
- [GitHub Workflow untuk Tim Indonesia](/github-workflow-indonesia)
- [Cara Setup SSH Key untuk GitHub](/setup-ssh-github)
- [Git Branching Strategy yang Efektif](/git-branching-strategy)
```

---

## Tips for Indonesian Audience

1. **Title yang specific**: "5 Git Tips" lebih baik dari "Git Tips"
2. **Intro yang hook**: Langsung tunjukin problem yang relate
3. **Code examples yang real**: Bukan contoh toy, tapi use case yang sering dihadapi
4. **Screenshots setiap 300-500 words**: Break up text, visual learners appreciate
5. **Bahasa casual tapi professional**: Seperti senior dev ngajarin junior
6. **Internal links**: Link ke artikel related, boost SEO
7. **CTA di akhir**: Suruh comment, share, atau baca artikel lain
