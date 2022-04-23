# minimum-typescript-env

### Getting Started

1. ```git clone https://github.com/Gityosan/minimum-typescript-env.git```
2. ```echo "# minimum-typescript-env" >> README.md```
3. ```yarn init -y```
4. ```yarn add -D gts```
5. ```npx gts init```
``` ```
``` ```

### About

- 最小構成のTypescript環境を調査するために作ったリポジトリです。
- まず、パッケージについて調査し、今後eslintの設定項目についても調査してまとめていく。

### Result

- gtsを使った環境構築では下記ライブラリが追加される。
  ```json
  "gts": "^3.1.0",
  "typescript": "^4.0.3",
  "@types/node": "^14.11.2"
  ```
- eslintとprettierの環境構築のために下記ライブラリを追加する。
  ```json
  "eslint": "^8.13.0",
  "eslint-config-prettier": "^8.5.0",
  "prettier": "^2.6.2"
  ```
- eslintをTypescript対応するために下記ライブラリを追加する。
  ```json
  "@typescript-eslint/eslint-plugin": "^4.2.0",
  "@typescript-eslint/parser": "^4.2.0"
  ```
  - gtsに内包されているためgts導入時には追加で入れる必要は無い。
- 下記を追加することでtypescriptをそのまま実行できる。
  ```json
  "ts-node": "^10.7.0",
  "ts-node-dev": "^1.1.8",
  ```