# LumaFader 韌體與 Editor

## 2026-10-07 更新

| 版本 | 配置 | 韌體 | 網頁 Editor |
|---|---|---|---|
| 4bank | 白紅黃綠四頁，每頁一個 bank；取消長按切 bank | [下載 4bank＋MIDI feedback](firmware-4bank-feedback.zip) | [開啟 4bank Editor](https://boringvery9-stack.github.io/LumaFader-v1.4_weifan-edit-20260805/4bank.html) |
| 16bank | 四頁，每頁四個 banks；保留原操作 | [下載 16bank＋MIDI feedback](firmware-16bank-feedback.zip) | [開啟 16bank Editor](https://boringvery9-stack.github.io/LumaFader-v1.4_weifan-edit-20260805/16bank.html) |

兩版均包含 fader MIDI CC 回傳燈號與 pickup 支援。Button 狀態回饋尚未加入。

## 安裝

適用已安裝 LumaFader v1.4 CircuitPython 與原 lib 的裝置。先備份，保留 lib、boot.py、settings.toml。
解壓縮後將 firmware 內的 .py 複製到裝置，code.py 最後複製，再重新插拔。
4bank 改版需要包內 settings.json，以套用新的四頁結構；會替換既有 mapping。
16bank 若要保留自己的 mapping，不要覆寫 settings.json。
Editor 必須與韌體版本配對。韌體包內附有設定與操作說明。

原 20260805 資料夾與原網頁入口均保留。
