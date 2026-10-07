# LumaFader 16bank MIDI feedback update — 2026-10-07

保留 4 Pages × 4 Banks（白／紅／黃／綠）的原有操作與 MIDI mapping。
新增 USB 與 TRS MIDI CC 回傳接收（所有 MIDI channels），以 CC＋channel 保存軟體參數目標值。
Fader 燈號顯示軟體回傳值；外部變更會重新啟用 pickup，避免推子直接跳值。
回傳接收不會 echo 發送。原本按鈕的 CC127→CC0 pulse 不變。

UA MIDI Control：啟用 LumaFader 的 MIDI input 與 MIDI output。
軟體回傳的 CC/channel 必須對應 editor 裡設定的 fader。

## 安裝
適用既有 LumaFader v1.4 CircuitPython 裝置（保留原 lib、boot.py、settings.toml）。
先備份装置。若要保留你自己的 mapping，不要覆寫 settings.json。
將包內 firmware/*.py（不含 boot.py）複製到裝置，code.py 最後複製；再重插裝置。
包內 settings.json 是縮減成 4bank 前的 16bank 設定快照，可選擇使用。
16bank editor：16bank.html。4bank editor 對應另一套四頁韌體，請勿混用。

本包來自加入 feedback 後、改為四頁前的已安裝版本；本次只整理成獨立下載包。
