https://qiita.com/EBIHARA_kenji/items/25e59f7132b96cb886f3

yarn add react react-dom redux react-redux
yarn add -D electron typescript eslint prettier eslint-config-prettier eslint-plugin-prettier webpack webpack-cli ts-loader
yarn add -D @types/react-dom`

electron: Electron ライブラリ
typescript: TypeScript コンパイラ
webpack: モジュールバンドラ JSが持たないモジュールの依存関係を解決するツール
ts-loader: webpackのTypeScript処理オプション・ライブラリ

yarn

yarn tsc --init

{
  "compilerOptions": {
    "target": "es2020", // Webpack で ES5に変換されるのでここでは最新の仕様
    "module": "commonjs",
    "jsx": "react",
    "sourceMap": true,
    "strict": true,
    "esModuleInterop": true,
    "sourceRoot": "./src",
    "forceConsistentCasingInFileNames": true
  },
  // コンパイル対象のファイル
  "files": [
    "src/main.ts" // メインプロセス用
    // レンダープロセスは Webpack でターゲットを指定するので、ここでは不要
  ]
}

/**/ サブディレクトリを再帰的にマッチ
* 0 個以上の文字列にマッチ
? 1 個の文字列にマッチ

yarn add eslint

yarn eslint --init

teramachishunsuke@Shunsuke-PC develop % yarn eslint --init
yarn run v1.22.10
warning ../package.json: No license field
$ /Users/teramachishunsuke/dev/develop/node_modules/.bin/eslint --init
✔ How would you like to use ESLint? · style
✔ What type of modules does your project use? · esm
✔ Which framework does your project use? · react
✔ Does your project use TypeScript? · No / Yes
✔ Where does your code run? · browser, node
✔ How would you like to define a style for your project? · guide
✔ Which style guide do you want to follow? · google
✔ What format do you want your config file to be in? · YAML
Checking peerDependencies of eslint-config-google@latest
The config that you've selected requires the following dependencies:

eslint-plugin-react@latest @typescript-eslint/eslint-plugin@latest eslint-config-google@latest eslint@>=5.16.0 @typescript-eslint/parser@latest
✔ Would you like to install them now with npm? · No / Yes
Installing eslint-plugin-react@latest, @typescript-eslint/eslint-plugin@latest, eslint-config-google@latest, eslint@>=5.16.0, @typescript-eslint/parser@latest


yarn add -D prettier eslint-config-prettier eslint-plugin-prettier

yarn add eslint-loader


yarn add html-webpack-plugin
yarn add -D prettier
yarn tsc
yarn webpack

yarn add typescript-fsa



