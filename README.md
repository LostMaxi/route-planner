# 動線規劃 Route Planner

基於 MapLibre GL 的交通動線規劃工具。

## 功能
- 在衛星地圖上繪製彩色動線
- L/F 狀態流動螞蟻線動畫
- 長方形車輛沿路徑行進動畫
- 地圖自由旋轉（羅盤控制）
- 精細縮放（0.25 級步進）
- **匯出 / 匯入 `.json` 工作文件**
- 本地儲存記錄（localStorage）
- 分享連結（URL hash）

## JSON 格式

```json
{
  "version": "1.0",
  "name": "規劃名稱",
  "createdAt": "2026-04-17T00:00:00.000Z",
  "map": { "center": [120.312, 22.676], "zoom": 16, "bearing": 0 },
  "flowParams": { "speed": 800, "weight": 4, "gap": 2, "opa": 0.9,
                  "carOn": true, "cspd": 1, "cnum": 1, "clen": 20, "cwid": 10 },
  "paths": [
    { "id": 1, "color": "#00e07a", "den": "L",
      "coords": [[120.31, 22.67], [120.32, 22.68]] }
  ]
}
```

## 部署

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/route-planner)
