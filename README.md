# 汉坦病毒全球爆发实时看板

## 项目简介
实时追踪全球汉坦病毒疫情数据的可视化看板，提供病例统计、地区分布、爆发预警和预防措施。

## 项目结构
```
hantavirus-dashboard/
├── backend/
│   └── data_collector.py    # 数据抓取脚本
├── frontend/
│   └── index.html           # 主页面
├── data/
│   └── latest_data.json     # 生成的数据文件
└── README.md
```

## 使用方法

### 1. 更新数据
```bash
cd backend
python3 data_collector.py
```

### 2. 本地预览
```bash
cd frontend
python3 -m http.server 8080
# 打开 http://localhost:8080
```

### 3. 部署到 GitHub Pages
```bash
git add -A
git commit -m "更新数据"
git push origin main
```

## 数据来源
- WHO (世界卫生组织)
- ECDC (欧洲疾病预防控制中心)
- CDC (美国疾病控制与预防中心)
- ProMED (国际传染病监测网络)

## 技术栈
- 前端: Leaflet.js (地图), HTML/CSS/JS
- 后端: Python 3.x
- 部署: GitHub Pages

## 许可证
MIT License
