# 狗运当骰互动幻灯片与技能卡控制台

适合桌面投影、桌游教学和公司活动使用的零依赖 HTML 页面。仓库目前包含完整的《狗运当骰》6 页互动幻灯片、两个独立互动页面，以及公司活动逆转技能控制台。

## 完整幻灯片

`spots-slides.html` 是主要入口，共 6 页：

1. 狗狗卡与后院：摇骰、自动演示和骰子拖放教学。
2. 技能卡控制台：六张技能卡、骨头标记和翻卡状态。
3. 开局初始化：个人组件、公共区和先手规则。
4. 回合选择：执行技能、狗狗计分及“可以／重复”关键词。
5. 骨头功能：使用时机与整批重掷规则。
6. 计分规则：填满、计分、翻面、补牌和获胜条件。

幻灯片支持右侧爪印导航、方向键、滚轮、触摸滑动、数字键 `1`–`6` 和全屏显示。

## 在线使用

### GitHub Pages

- 完整 6 页互动幻灯片：<https://pnmiracle.github.io/spots-skill-console/spots-slides.html>
- 骰子放置互动教学：<https://pnmiracle.github.io/spots-skill-console/dice-placement-guide.html>
- 狗运当骰技能卡控制台：<https://pnmiracle.github.io/spots-skill-console/>
- 公司活动逆转技能控制台：<https://pnmiracle.github.io/spots-skill-console/fate-skill-console.html>

### Vercel

- 完整 6 页互动幻灯片：<https://spots-slides-vercel-20260701.vercel.app>
- 狗运当骰技能卡控制台：<https://deploy-spots.vercel.app>
- 公司活动逆转技能控制台：<https://deploy-fate.vercel.app>

## 本地预览

在仓库根目录运行：

```bash
python3 -m http.server 8765
```

然后打开：

- 完整幻灯片：<http://127.0.0.1:8765/spots-slides.html>
- 技能卡控制台：<http://127.0.0.1:8765/>
- 骰子放置教学：<http://127.0.0.1:8765/dice-placement-guide.html>

使用 HTTP 预览可以保证幻灯片中的内嵌页面和交互正常加载。

## 页面操作

### 完整幻灯片

- 点击右侧爪印或上下按钮切换页面。
- 使用方向键、滚轮、触摸滑动或数字键 `1`–`6` 换页。
- 按 `F` 进入或退出全屏。

### 狗运当骰技能卡控制台

- 点击技能卡切换可用/已使用状态。
- 按 `1`–`6` 快速翻转对应技能卡。
- 按 `R` 重置技能板，按 `F` 进入或退出全屏。
- 拖动骨头标记到技能卡或顶部放置区。

### 公司活动逆转技能控制台

- 点击技能卡切换待命/已使用状态。
- 按 `1`–`0` 快速触发对应技能卡。
- 按 `R` 全部重新充能，按 `F` 进入或退出全屏。
- 点击顶部技能类型筛选按钮，可只查看某一类技能。

## 主要文件

- `spots-slides.html`：6 页互动幻灯片总入口。
- `dice-placement-guide.html`：狗狗卡、后院和骰子放置教学。
- `index.html`：狗运当骰技能卡控制台。
- `fate-skill-console.html`：公司活动逆转技能控制台。
- `assets/`：技能图标与教学示例图片。
