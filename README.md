### 環境構築
プロジェクトディレクトリを作成
```
mkdir <ProjectName> && cd <ProjectName>
```
色々ダウンロード
```bash
npm i three @pixiv/three-vrm
npm i -D webpack webpack-cli typescript ts-loader webpack-dev-server
npm i --save-dev @types/three
```
エラーが起こる場合
```diff
- npm i -D webpack webpack-cli typescript ts-loader webpack-dev-server
+ npm i -D webpack webpack-cli typescript ts-loader webpack-dev-server --legacy-peer-deps
- npm i --save-dev @types/three
+ npm i --save-dev @types/three --legacy-peer-deps
```
### ブラウザで表示
TypeScriptをコンパイル
```
npm run build
```
実行
```
npm run dev
```

##### 参考
https://scrapbox.io/ke456memo/%2324_pixiv%2Fthree-vrm_+_TypeScript%E3%81%AE%E3%83%86%E3%83%B3%E3%83%97%E3%83%AC%E3%83%BC%E3%83%88%E3%82%92%E4%BD%9C%E3%82%8B<br>
\- https://github.com/Keshigom/threeVrmTemplate/tree/master
##### 変更点
webpackage v-5対応
