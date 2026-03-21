---
type: note
tags:
  - claude_code
  - 使用体验
date_created: 2026-03-21
date_updated: 2026-03-21
---

# Claude Code 使用体验

记录使用 Claude Code 的心得、技巧和问题解决方案。

---

## 2026-03-20

### 初次体验：ccswitch + 智谱 GLM

今天参考论坛教程，尝试使用 **ccswitch** 搭配 **智谱 GLM** 模型来体验 Claude Code。

**整体感受：还不错！**

- 响应速度可以接受
- 基本功能都能正常使用
- 对于日常编程辅助来说够用

**存在的问题：**
- 免费 token 额度较少
- 付费版本比较火爆，经常抢不到

---

## 2026-03-21

### 切换到 Minimax 免费 API

今天改用 **Minimax 免费 API**，尝试替代方案。

（待补充使用体验...）

---

## 一些问题与解答

### Q: 对话历史不保留？
**现象**：每次启动 Claude Code 都是新会话，之前的对话内容丢失。

**原因**：Claude Code 不会自动保存会话历史。

**解决方案**：
- 保持会话不断开
- 重要内容手动保存到笔记中
- 使用 memory/ 目录保存关键要点

### Q: WebSearch API 报错？

**现象**：使用 WebSearch 时返回 API Error 400。

**原因**：中间模型（ccswitch/minimax）可能没有配置 WebSearch 功能权限，这是功能阉割导致的。

**解决方案**：
- 使用官方 Anthropic API（功能完整但较贵）
- 接受中间模型功能受限

### Q: 中间模型 API vs 官方 API？

|  | 中间模型 (ccswitch/minimax) | 官方 API |
|---|---|---|
| 来源 | 第三方转发 | Anthropic 直营 |
| 费用 | 便宜/免费 | 较贵 |
| 功能 | 部分功能受限 | 完整功能 |
| 速度 | 取决于中间层 | 稳定 |

---

## 📝 待记录

- [ ] Minimax 免费 API 的具体使用体验
- [ ] token 消耗情况
- [ ] 遇到的坑和解决方案
- [ ] 推荐的配置组合
