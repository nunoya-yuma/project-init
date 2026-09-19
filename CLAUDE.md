# project-init

## スコープ
- このツールが書き込む対象は `.private-scratch/`（個人用・非公開）に限定する。
  新規プロジェクト作成時だけでなく、既存プロジェクトへの参画時にも使うため、
  対象プロジェクトの共有・トラッキングされるファイル（.gitignore、
  .editorconfig、git hooksなど）には書き込まない。
- 新機能を検討する際は、先に個人のdotfilesリポジトリ（GitHub:
  `nunoya-yuma/dotfiles`。ローカルの配置場所は固定していないので、
  見当たらなければユーザーに確認する）と役割が被っていないか確認する。
  特に `core.hooksPath` とgitのグローバルexcludesファイルは、
  dotfilesリポジトリの `git/gitconfig` / `git/ignore` でマシン全体に
  設定済みのことが多いため、project-init側でリポジトリローカルに同種の
  設定を行うと上書き・衝突する可能性がある。
