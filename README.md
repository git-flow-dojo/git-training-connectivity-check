# 接続確認用リポジトリ（Git・GitHub Flow 研修 事前準備）

研修当日の `git push` の認証が事前に通るかを確認する専用リポジトリです。
研修の教材・演習内容は含みません。手順の詳細と認証の方法（Windows はブラウザで
ログイン、Mac も Git Credential Manager でブラウザからログイン）は「研修事前準備_受講者」の ③-2 をご覧ください。

`<ユーザー名>` はご自身の GitHub のユーザー名に置き換えてください。

    cd ~
    git clone https://github.com/git-flow-dojo/git-training-connectivity-check.git
    cd git-training-connectivity-check
    code <ユーザー名>.html          # 中身は空でも可。保存して閉じる
    git add <ユーザー名>.html
    git commit -m "接続確認 <ユーザー名>"
    git push

## 成功の判定

- [ ] `git push` が `Authentication failed` などのエラーなく完了した
- [ ] GitHub 上（`main`）に `<ユーザー名>.html` が表示される
- [ ] そのコミットの作者欄に、本名ではなく GitHub のユーザー名が表示される

できたら準備状況シートの「接続確認」にチェックを入れてください。
