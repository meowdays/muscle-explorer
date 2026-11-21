# Muscle Explorer

繁體中文介面的靜態 3D 人體肌肉探索工具，可自行部署到 GitHub Pages。

## 操作
- 單指拖曳：旋轉模型
- 雙指捏合：縮放
- 點一下肌肉：選取及查看中英文名稱
- 快速連點兩下：聚焦該肌肉
- 搜尋肌肉、單獨顯示、隱藏、還原
- 正面／背面／左側／右側預設視角
- 臀部及背部深層顯示選項

## 部署到 GitHub Pages
1. 解壓縮 ZIP。
2. 將 `muscle-explorer` 資料夾**內部所有檔案及資料夾**上傳到 GitHub repository 的 Pages 發佈根目錄。
3. 在 repository 的 Settings → Pages 選擇發佈來源。
4. 用 HTTPS 網址開啟。

## 重要：3D 模型及網絡依賴
此 ZIP 包含網站程式、介面、圖示及設定，但**沒有把 GLB 3D 模型或 Three.js/Draco 函式庫打包在內**。模型會由下列公開來源載入，Three.js 及 Draco decoder 亦由 CDN 載入，因此首次載入模型時必須連接互聯網：
- Muscle model: https://github.com/SeemaBansal1/3d-human-body-anatomy
- Three.js r180: https://cdn.jsdelivr.net/npm/three@0.180.0/
- Draco decoder: https://www.gstatic.com/draco/versioned/decoders/1.5.7/

如果上述第三方服務或網絡不可用，3D 模型便不能載入。此版本不應描述為完全離線或所有資產已內置。

## 模型授權及致謝
肌肉及骨骼模型來源項目使用 Z-Anatomy / BodyParts3D 衍生資料。上游 README 標示 Z-Anatomy 為 CC BY-SA 4.0，並列出 BodyParts3D 的來源及授權。請保留上游署名並在再散布模型時遵守相同授權條款。詳見 `CREDITS.md` 及上游 repository 的最新授權檔案。

本工具只供解剖學參考，不作醫療診斷。
