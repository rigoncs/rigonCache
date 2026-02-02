# rigonCache

rigonCache 是一个基于 **C++20** 的缓存系统练手项目，目标是通过实现多种经典缓存替换算法，系统性地提升对 **C++ 语言、STL、面向对象设计以及工程化构建流程** 的理解。

该项目以“**边学边造轮子**”为导向，强调：
- 清晰的接口设计
- 可扩展的缓存策略
- 规范的工程结构

适合作为：
- C++ 进阶学习项目  
- 数据结构 / 缓存算法实践  
- 面试或技术展示项目  

---

## ✨ 项目特性

- 使用 **C++20** 标准
- 基于 **CMake** 构建
- 面向接口编程，支持多缓存策略
- 模块化设计，易于扩展
- 提供统一测试入口，便于验证与对比

---

## 🧠 缓存策略实现情况

- [x] LRU（Least Recently Used）
- [x] LFU（Least Frequently Used）
- [ ] ARC（Adaptive Replacement Cache，计划中）

> ARC 是一种自适应缓存替换算法，结合了 LRU 和 LFU 的优点，作为本项目的进阶实现目标。

---

## 📁 项目结构说明

```text
.
├── CMakeLists.txt          # CMake 构建配置
├── README.md               # 项目说明文档
├── RICachePolicy.h         # 缓存策略接口（抽象基类）
├── RLruCache.h             # LRU 缓存实现
├── RLfuCache.h            # LFU 缓存实现
├── RArcCache/              # ARC 缓存实现
├── testAllCachePolicy.cpp  # 各缓存策略的测试入口
├── build/                  # 构建目录（不纳入版本控制）
