# 儿童英语词汇卡

包含 2,023 张 JPEG 词汇卡，支持英文和中文搜索、单词选择以及上一张和下一张浏览。页面适配手机屏幕。

## 本地查看

在仓库目录运行 `python3 -m http.server 8000`，然后打开 http://localhost:8000。

## 发布

在 GitHub 仓库 Settings → Pages 中将 Source 设为 GitHub Actions。推送到 main 后自动部署，也可以在 Actions 中手动运行 Deploy vocabulary cards。

部署成功后的地址为 https://rubinxin.github.io/vocabulary-cards/。

## 更新词卡

`words.js` 中每条记录包含英文和中文释义，记录的数组下标对应 `cards/<下标>.jpg`。新增或重新排序词表时，须同步对应图片，确保文件名与数组下标一致。发布前核对每条记录都有对应 JPEG。
