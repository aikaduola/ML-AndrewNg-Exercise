# ML-AndrewNg-Exercise

> 吴恩达（Andrew Ng）机器学习课程课后练习题与 Jupyter 实验环境

本项目用于整理和复现吴恩达机器学习课程配套的课后练习题（Exercise），包含实验数据集、机器学习算法实现以及 Jupyter Notebook 实验环境。

---

## 1. 项目简介

### 项目用途

* 学习吴恩达机器学习课程
* 完成课程配套课后练习题
* 运行 Jupyter Notebook 实验
* 学习和实践经典机器学习算法
* 复现实验结果

### 项目结构

| 文件 / 目录                   | 说明                       |
| ------------------------- | ------------------------ |
| `data`                    | 实验所需的数据集                 |
| `models`                  | 机器学习算法及实验辅助代码            |
| `requirements.txt`        | Python 项目依赖              |
| `.pre-commit-config.yaml` | Git 提交检查及代码格式化配置         |
| `.venv`                   | 项目专属 Python 虚拟环境，不纳入 Git |

---

## 2. 环境要求

开始使用项目之前，请确认本地已安装：

* **Python 3.11.x**（推荐 3.11.9）
* **Git**

检查版本：

```bash
python --version
git --version
```

---

## 3. 环境初始化

首次使用项目时，在项目根目录按照以下步骤执行。

### ① 克隆项目

```bash
git clone https://github.com/aikaduola/ML-AndrewNg-Exercise.git
cd ML-AndrewNg-Exercise
```

### ② 创建虚拟环境

```bash
python -m venv .venv
```

### ③ 激活虚拟环境

**Windows CMD：**

```cmd
.venv\Scripts\activate
```

**Windows Git Bash：**

```bash
source .venv/Scripts/activate
```

激活成功后，终端前面会出现：

```text
(.venv)
```

### ④ 安装项目依赖

```bash
pip install -r requirements.txt
```

### ⑤ 配置 pre-commit

```bash
pre-commit install
```

### ⑥ 执行首次代码检查

```bash
pre-commit run --all-files
```

检查全部通过后，项目环境初始化完成。

### ⑦ 启动 Jupyter Notebook

```bash
jupyter notebook
```

浏览器打开 Jupyter 后，即可选择对应的 Notebook 开始实验。

---

## 4. 日常使用

完成首次初始化后，每次使用项目只需要：

**Windows CMD：**

```cmd
cd ML-AndrewNg-Exercise
.venv\Scripts\activate
jupyter notebook
```

**Windows Git Bash：**

```bash
cd ML-AndrewNg-Exercise
source .venv/Scripts/activate
jupyter notebook
```

完成实验后退出虚拟环境：

```bash
deactivate
```

---

## 5. Git 提交

修改代码后，提交前建议执行：

```bash
pre-commit run --all-files
```

检查通过后：

```bash
git add .
git commit -m "提交说明"
```

项目已配置 `pre-commit`，执行 `git commit` 时也会自动进行代码检查。

---

## 6. 常用命令

| 操作             | 命令                                |
| -------------- | --------------------------------- |
| 创建虚拟环境         | `python -m venv .venv`            |
| 激活环境（CMD）      | `.venv\Scripts\activate`          |
| 激活环境（Git Bash） | `source .venv/Scripts/activate`   |
| 安装依赖           | `pip install -r requirements.txt` |
| 安装 pre-commit  | `pre-commit install`              |
| 全量代码检查         | `pre-commit run --all-files`      |
| 启动 Jupyter     | `jupyter notebook`                |
| 退出虚拟环境         | `deactivate`                      |

---

## 7. 注意事项

* 建议始终在 `.venv` 虚拟环境中运行项目。
* `.venv` 为本地开发环境，不需要提交到 Git。
* `requirements.txt` 发生变化后，需要重新执行：

```bash
pip install -r requirements.txt
```

* 如果 `pre-commit` 检查失败，请根据终端提示修复后重新执行：

```bash
pre-commit run --all-files
```

---

## 8. 开始学习

环境配置完成后，启动 Jupyter Notebook：

```bash
jupyter notebook
```

选择对应课程章节的 Notebook，即可开始吴恩达机器学习课程实验。

> **Enjoy Machine Learning! 🚀**
