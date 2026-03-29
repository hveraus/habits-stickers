# HabitsSticker — Sticker Pack

贴纸资源库，供 HabitsSticker App 使用。

## 结构

```
stickers/
  common/       普通贴纸 (70%)
  rare/         稀有贴纸 (20%)
  super_rare/   超稀有贴纸 (8%)
  legendary/    传说贴纸 (2%)
manifest.json   贴纸目录（App 拉取此文件获取贴纸列表）
```

## 图片规范

- 格式：PNG，透明背景
- 尺寸：256 × 256 px
- 文件名：与 `manifest.json` 中的 `id` 字段一致，如 `cat_smile.png`

## manifest.json 格式

```json
{
  "version": 1,
  "stickers": [
    { "id": "cat_smile", "name": "微笑猫咪", "rarity": "普通", "theme": "动物" }
  ]
}
```

`rarity` 取值：`普通` / `稀有` / `超稀有` / `传说`
