# LumaFader Firmware & Editor / 韌體與編輯器

## English

### Versions

Two independent versions are available. Match the editor to your firmware.

| Version | Layout | Firmware | Web editor |
|---|---|---|---|
| 4bank | Four color pages, one bank per page; single-button bank switching removed | [Download 4bank feedback firmware](firmware-4bank-feedback.zip) | [4bank editor](https://boringvery9-stack.github.io/LumaFader-v1.4_weifan-edit-20260805/4bank.html) |
| 16bank | Four pages, four banks per page; original controls preserved | [Download 16bank feedback firmware](firmware-16bank-feedback.zip) | [16bank editor](https://boringvery9-stack.github.io/LumaFader-v1.4_weifan-edit-20260805/16bank.html) |

Both versions include MIDI CC feedback for fader LEDs and pickup. To display a parameter’s current value, the control software must send matching MIDI CC feedback to LumaFader; outgoing controller messages alone cannot provide this state. Button state feedback is not included yet.

### Installation

Install on an existing LumaFader v1.4 CircuitPython device with the original libraries. Back up first and retain `lib`, `boot.py`, and `settings.toml`. Copy the Python files from `firmware`, copy `code.py` last, then reconnect USB.

For the 4bank migration, also copy the included `settings.json`; it replaces the current mappings with the four-page layout. For 16bank, keep your existing `settings.json` to preserve your mappings. See the README inside each archive for controls and setup.

The original 20260805 folder and original editor URL are preserved.

### Controls

Hold the bottom button, then press the top button to go to the next page. Hold the top button, then press the bottom button to go to the previous page.

- **4bank:** A single-button hold does not switch banks.
- **16bank:** Hold a single button to switch banks.

## 中文

### 版本

| 版本 | 配置 | 韌體 | 網頁 Editor |
|---|---|---|---|
| 4bank | 白紅黃綠四頁，每頁一個 bank；取消長按切 bank | [下載 4bank＋MIDI feedback](firmware-4bank-feedback.zip) | [開啟 4bank Editor](https://boringvery9-stack.github.io/LumaFader-v1.4_weifan-edit-20260805/4bank.html) |
| 16bank | 四頁，每頁四個 banks；保留原操作 | [下載 16bank＋MIDI feedback](firmware-16bank-feedback.zip) | [開啟 16bank Editor](https://boringvery9-stack.github.io/LumaFader-v1.4_weifan-edit-20260805/16bank.html) |

兩版均包含 fader MIDI CC 回傳燈號與 pickup 支援。若要顯示參數的目前數值，控制軟體必須將對應的 MIDI CC 回傳給 LumaFader；只有控制器送出的訊息無法取得軟體狀態。Button 狀態回饋尚未加入。

### 安裝

適用已安裝 LumaFader v1.4 CircuitPython 與原 lib 的裝置。先備份，保留 lib、boot.py、settings.toml。
解壓縮後將 firmware 內的 .py 複製到裝置，code.py 最後複製，再重新插拔。
4bank 改版需要包內 settings.json，以套用新的四頁結構；會替換既有 mapping。
16bank 若要保留自己的 mapping，不要覆寫 settings.json。
Editor 必須與韌體版本配對。韌體包內附有設定與操作說明。

原 20260805 資料夾與原網頁入口均保留。


### 操作

按住最下鍵再按最上鍵：下一頁。按住最上鍵再按最下鍵：前一頁。

- **4bank：** 長按單一按鍵不切換 bank。
- **16bank：** 長按單一按鍵切換 bank。

## Original design / 原始設計

Original MIDI controller design by **DJBajaBlast**. [Buy the controller ↗](https://www.etsy.com/listing/1872693350/lumafader-68-midi-controller-rgb-faders)
