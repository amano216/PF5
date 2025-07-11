# 禅 × 宇宙 - Zen Galaxy Interactive Experience

![Zen Galaxy](https://img.shields.io/badge/Three.js-r128-black?style=flat-square)
![GSAP](https://img.shields.io/badge/GSAP-3.12.2-88CE02?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

## 🌌 Overview

極限までシンプルを追求した禅の精神と、無限に広がる銀河の美しさを融合させたインタラクティブな体験。10万個の星が織りなす宇宙空間で、静寂と無限を感じる。

[Live Demo](https://amano216.github.io/PF5/)

## 🎯 Vibe Coding Prompt

以下のプロンプトで、このサイトの雰囲気を再現できます：

```
禅の精神と宇宙の無限性を融合させた、究極にミニマルでスタイリッシュなインタラクティブサイトを作って。

要件：
- 背景は完全な黒（#000）で、10万個の粒子で渦巻き銀河を3Dで表現
- 中心に巨大な「禅」の文字を、崩れた草書体風フォント（Yuji Syuku）で配置
- 文字は透明度15%、強いグロー効果で銀河と一体化
- 文字は45度回転しながらスケールアップして登場、その後エコーエフェクト
- マウスの動きに微妙に反応するカメラ
- クリックで光の波紋と銀河の回転加速
- 右上に「銀河」「虚空」「無限」の3つのビューモード
- 'z'キーで究極禅モード（UIを消して星を小さく）
- 全体的に静寂と動きのバランスを保つ

技術：
- Three.js（パーティクルシステム）
- GSAP（スムーズアニメーション）
- 日本語フォントとSpace Groteskの組み合わせ
- mix-blend-modeでテキストと背景を融合

色彩：
- 銀河の内側：#ff6030（オレンジ）
- 銀河の外側：#1b3984（深い青）
- テキスト：白（透明度調整）
```

## 🛠 Technical Specifications

### Dependencies
- **Three.js r128** - 3D graphics and particle system
- **GSAP 3.12.2** - Smooth animations and transitions
- **Google Fonts** - Yuji Syuku (Japanese), Space Grotesk (English)

### Key Features
1. **3D Galaxy Particle System**
   - 100,000 particles forming a spiral galaxy
   - Dynamic color gradient from center to edge
   - Continuous rotation with mouse interaction

2. **Typography Animation**
   - Scale and rotate entrance animation
   - Echo effect creating depth
   - Blur transitions for mystical feel

3. **Interactive Elements**
   - Mouse-following camera movement
   - Click ripple effects
   - Three view modes (Galaxy/Void/Infinity)
   - Zen mode toggle (press 'z')

### Performance Optimizations
- Efficient particle rendering with BufferGeometry
- Additive blending for luminous effect
- Responsive design with dynamic resizing

## 📁 Project Structure

```
PF5/
├── index.html      # Single-file application
└── README.md       # This file
```

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/amano216/PF5.git
cd PF5
```

2. Open `index.html` in a modern web browser
   - Or use a local server: `python -m http.server 8000`

## 🎨 Customization

### Galaxy Parameters
```javascript
const parameters = {
    count: 100000,        // Number of stars
    size: 0.01,          // Star size
    radius: 5,           // Galaxy radius
    branches: 5,         // Spiral arms
    spin: 1,             // Spiral intensity
    randomness: 0.2,     // Star scatter
    insideColor: '#ff6030',
    outsideColor: '#1b3984'
};
```

### Animation Timing
- Zen title reveal: 2s cubic-bezier
- Echo effect: 4s cycle, 2s delay
- Galaxy rotation: 0.05 rad/s
- Camera float: Sine wave modulation

## 🎮 Controls

| Action | Effect |
|--------|--------|
| Mouse Move | Camera follows cursor |
| Click | Ripple effect + Galaxy spin |
| 銀河 Button | Default galaxy view |
| 虚空 Button | Front view into the void |
| 無限 Button | Top-down infinity view |
| Press 'Z' | Toggle zen mode |

## 🧘 Philosophy

このプロジェクトは、東洋の禅思想と西洋のテクノロジーの融合を表現しています。シンプルさの中に無限の複雑さを、静寂の中に永遠の動きを見出す。

> "山は山である、水は水である" - 道元禅師

## 📜 License

MIT License - feel free to use this code for your own cosmic zen journey.

## 🙏 Credits

Created with 🤖 Claude Code

---

*Experience the void. Embrace the infinite. Find your zen.*