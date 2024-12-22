# pplx-api-trial

perplexity api (pplx-api) を試してみた際の記録です。

## 実行に必要なもの

- direnv
- uv
- Visual Studio Code (必要に応じて)

## 準備

### API Key の準備

.envrc を作成し、取得した Perplexity API、OpenAI API の API Key で置き換える。

```bash
cp .envrc.sample .envrc
```

Perplexity API の API Key の取得方法

- <https://docs.perplexity.ai/guides/getting-started#generate-an-api-key>

OpenAI API の API Key の取得方法

- <https://platform.openai.com/docs/quickstart#create-and-export-an-api-key>

## 依存関係の準備

```bash
uv sync --frozen
```

## 実行

Visual Studio Code で .ipynb ファイルを開き、実行する。

Visual Studio Code を使わない場合、以下のコマンドでも実行できそうです。

```bash
uv run --with jupyter jupyter lab
```
