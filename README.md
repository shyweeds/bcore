# OSTEP + CSAPP + OSDev Wiki 最小学习路径（写 Toy OS）

## 一、目标
能够基于 OSDev Wiki 写一个 toy operating system（bootable + 内存管理 + 基础进程）

---

## 二、CSAPP 最小必做内容

### 必做
- ✔ malloc lab  
  - 理解 heap / free list / fragmentation  
  - 用于实现 kernel memory allocator

### 建议做
- ✔ shell lab  
  - 理解 fork / exec / wait  
  - 帮助理解进程模型

### 可忽略
- cache lab（性能优化方向）
- proxy lab（网络应用层）

---

## 三、OSTEP 最小必做内容

### 必须掌握（核心 OS 概念）

#### 1. Process + Scheduling
- process abstraction
- context switch
- scheduling policy

#### 2. Virtual Memory
- paging
- address translation
- page table

#### 3. Concurrency
- locks
- condition variables
- race condition 基础

### 建议了解
- file system（inode / block / directory）
- I/O abstraction

### lab 建议
- scheduling lab（必须）
- VM lab（必须）
- concurrency lab（建议）

---

## 四、OSDev Wiki 必备补充知识

### 必须掌握
- boot process（BIOS/UEFI → kernel）
- x86 protected mode / long mode
- GDT / IDT
- paging enable
- interrupt handling

### 强烈建议
- ELF format
- linker script
- QEMU + GDB 调试流程

---

## 五、最小可行学习集合（MVP）

如果目标是尽快写 OS：

### CSAPP
- malloc lab

### OSTEP
- process + scheduling
- virtual memory
- concurrency basics

### OSDev Wiki
- boot loader
- paging
- interrupt system

---

## 六、推荐实践顺序（关键）

1. CSAPP malloc lab → 写 kernel heap
2. OSTEP VM → 实现 paging
3. OSTEP process → 简单 scheduler
4. OSDev Wiki → boot + interrupt
5. 整合成 toy OS

---

## 七、核心原则

- 不要“学完再做”，边学边写 kernel
- 每学一个概念 → 立刻在 OS 里实现
- OS = 工程拼装，不是课程学习

---
