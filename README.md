# AI-colab-video

用 Google Colab（Colab CLI）生成 AI 影片的專案。

## mireva_ad — MIRÉVA 晨霧光透精華（虛構品牌）30 秒廣告

- 16:9、6 鏡、無台詞，品牌字卡與 AI 標示在後製疊加。
- 流程：[shanshiba-workflow-colab](https://github.com/mathruffian-dot/shanshiba-workflow-colab) 的 `pipeline/template_local`（Qwen-Image-Edit 首幀 → MiniMax H3 影片 → MiniMax-Music3 配樂）。
- 用法：把 `mireva_ad/` 放進 shanshiba repo 的 `pipeline/`，再執行
  `python cloud/colab_h3.py film pipeline/mireva_ad chars masters frames`，
  人工確認首幀後 `... film pipeline/mireva_ad h3 edl music cut review`。
- `out/chars/mirei.png`：角色參考（取自個人角色設定圖主視覺）。

注意：MiniMax H3 授權排除美國／歐盟／英國／南韓；Qwen-Image、Breeze TTS 限非商業用途。
