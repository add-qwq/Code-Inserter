# English:
# Umami Analytics Code Injector  

![GitHub release (latest by date)](https://img.shields.io/github/v/release/add-qwq/Code-Inserter?style=flat-square)  
![GitHub stars](https://img.shields.io/github/stars/add-qwq/Code-Inserter?style=flat-square)  
![Python version](https://img.shields.io/badge/Python-3.0%2B-blue?style=flat-square)  
![License](https://img.shields.io/github/license/add-qwq/Code-Inserter?style=flat-square)  

As we all know, there's a great project on GitHub: [https://github.com/umami-software/umami](https://github.com/umami-software/umami).  

However, here's an issue: if your website is already built and you want to use Umami's statistics, you need to insert the code provided by Umami Cloud into the **head** tag of your web files.  

Manually modifying each file is not feasible, so I've developed this small tool that can automatically inject Umami's statistical code into your web files.  

Of course, I haven't covered other types yet, so it only supports **.php** and **.html** (or **.htm**) files.  

Just enter your website ID (i.e., the **data-website-id** parameter in Umami's statistical code) in the GUI, select your local web files, click "Inject," and you're done!  

So, if you need it, feel free to scroll down for a detailed introduction to the project

---

**Unofficial tool** to batch inject Umami analytics tracking code into HTML/PHP files. Designed to simplify adding [Umami](https://github.com/umami-software/umami) tracking to existing websites by automatically inserting the script into the **<head>** section of multiple files at once.  


## 🌟 Key Features  
- **Batch Injection**: Process multiple HTML/.htm/.php files simultaneously.  
- **Auto Backup**: Creates **.bak** backups of original files before modifying them.  
- **Multi-Website Support**: Inject codes for multiple Umami website IDs in one go.  
- **Bilingual Interface**: Switch between English and Simplified Chinese directly in the UI.  
- **Progress Tracking**: Real-time progress bar and status updates for each file.  


## 🚀 Quick Start  

### Option 1: Download Prebuilt EXE (Recommended)  
No Python setup needed:  
1. Go to the [Releases page](https://github.com/add-qwq/Code-Inserter/releases).  
2. Download **Code-Inserter-EXE.zip** and extract it.  
3. Run **Code-Inserter.exe** (auto-detects system language, or use language toggle in UI).  

**Security Note**: If you prefer to build from source for verification, see Option 2 below.  


### Option 2: Run from Source Code  
For developers or users who prefer to build locally:  

#### Prerequisites  
- Python 3.0+  
- Required packages:  
  ```bash  
  pip install pyside6  
  ```  

#### Steps  
1. Download the source code:  
   - Click **Code → Download ZIP** on the [GitHub repo](https://github.com/add-qwq/Code-Inserter).  
   - Extract the ZIP file.  

2. Run the program:  
   ```bash  
   cd Code-Inserter  # Navigate to the project folder  
   python Code-Inserter.py  # Launch the application  
   ```  


## 📦 Build EXE from Source (for verification)  
If you do not trust the prebuilt EXE files, you can compile the source code into an executable yourself for security purposes:  

```bash  
# Install pyinstaller if not done already  
pip install pyinstaller  

# Navigate to the project folder  
cd Code-Inserter  

# Create the EXE (Windows)  
pyinstaller -w -F --name "Code-Inserter" Code-Inserter.py  

# Parameters:  
# -w: Hide console window (GUI mode).  
# -F: Generate a single EXE file.  
# --name: Set the output file name.  
```  

**For macOS/Linux**: Use the same command, replacing **;** with **:** in file paths if needed.  


## 🖥 Interface Overview  
![English Interface](https://github.com/add-qwq/Code-Inserter/blob/main/Code-Inserter-EN.png?raw=true)  
*(Switch to Chinese via the **"切换到中文"** button in the UI.)*  


## 📘 How to Use  

### Step 1: Enter Website IDs  
1. In the text area labeled **"Website IDs"**, enter your Umami **data-website-id** values (one per line).  
   - Example:  
     ```  
     your-website-id-1  
     your-website-id-2  
     ```  

### Step 2: Select Files  
1. Click **"Select Files"** to choose HTML/.htm/.php files from your local directory.  
2. Use **"Remove Selected Files"** or **"Clear File List"** to manage the file queue.  

### Step 3: Inject Code  
1. Click **"Inject Analytics Code"**.  
2. Confirm the operation (backups will be created automatically).  
3. Monitor progress in the status bar and progress bar.  

### Post-Injection  
- A success message will appear if all files are processed.  
- For partial failures, check the status bar for details.  


## 📜 License  
This project is licensed under the [Apache License 2.0](https://github.com/add-qwq/Code-Inserter/blob/main/LICENSE).  


## 🙋 Feedback  
- **Issue Tracking**: Report bugs or request features on the [Issues page](https://github.com/add-qwq/Code-Inserter/issues).  
- **Contributions**: Fork the repo and submit pull requests for improvements.  


---


# 中文：
# Umami统计代码注入工具  

![GitHub release (latest by date)](https://img.shields.io/github/v/release/add-qwq/Code-Inserter?style=flat-square)  
![GitHub stars](https://img.shields.io/github/stars/add-qwq/Code-Inserter?style=flat-square)  
![Python version](https://img.shields.io/badge/Python-3.0%2B-blue?style=flat-square)  
![License](https://img.shields.io/github/license/add-qwq/Code-Inserter?style=flat-square)  

众所周知，GitHub 上存在一个很棒的项目：[https://github.com/umami-software/umami](https://github.com/umami-software/umami)  

不过有一个问题，如果你的网站已经编写好了，但是你想要使用 umami 的统计，就需要在你的 web 文件里的 **head** 标签内插入 umami cloud 提供的代码

而一个个更改文件是不现实的，所以我编写了这个小工具，它可以帮你自动在你的 web 文件里注入 umami 的统计代码

当然，我没有接触过其他类型，所以只支持 **.php** 和 **.html**（也可以是 **.htm**） 

只需要在 GUI 输入你的网站 id（也就是 umami 的统计代码里的 **data-website-id** 参数），然后选中你的本地 web 文件，点击注入，完成！  

所以，如果你有需要，可以看看往下继续查看该项目的详细介绍

---

**非官方工具**，用于批量向HTML/PHP文件注入Umami统计代码。解决手动在大量网页文件中插入统计代码的痛点，自动将Umami跟踪脚本插入到文件的**<head>**标签中，支持一次处理多个文件


## 🌟 核心功能  
- **批量注入**：同时处理多个HTML/.htm/.php文件。  
- **自动备份**：修改前自动创建原文件的**.bak**备份。  
- **多网站支持**：支持同时注入多个Umami网站ID的统计代码  
- **双语界面**：直接在界面中切换英文/简体中文。  
- **进度监控**：实时显示每个文件的处理进度和状态  


## 🚀 快速开始  

### 方式 1：下载预编译EXE（推荐）  
无需安装Python环境：  
1. 前往 [Releases 页面](https://github.com/add-qwq/Code-Inserter/releases) 
2. 下载 **Code-Inserter-EXE.zip** 并解压  
3. 运行 **Code-Inserter.exe**（程序会自动检测系统语言，也可在界面中手动切换）  

**安全提示**：若您对预编译文件的安全性存疑，可通过下方方式2下载源码自行编译  


### 方式 2：从源代码运行  
适合开发者或需要自主编译的用户：  

#### 环境要求  
- Python 3.0+  
- 安装依赖：  
  ```bash  
  pip install pyside6  
  ```  

#### 步骤  
1. 下载源代码：  
   - 在 [GitHub 仓库](https://github.com/add-qwq/Code-Inserter) 点击 **Code → 下载 ZIP**  
   - 解压下载的ZIP文件。  

2. 运行程序：  
   ```bash  
   cd Code-Inserter  # 进入项目目录  
   python Code-Inserter.py  # 启动程序  
   ```  


## 📦 从源码编译EXE（自主验证）  
如果您不信任我们提供的预编译EXE文件，可以下载源代码后自行编译为可执行文件，确保安全性：  

```bash  
# 先安装pyinstaller  
pip install pyinstaller  

# 进入项目目录  
cd Code-Inserter  

# 打包EXE（Windows）  
pyinstaller -w -F --name "Code-Inserter" Code-Inserter.py  

# 参数说明：  
# -w：隐藏控制台窗口（图形界面模式）  
# -F：生成单个EXE文件（而非目录）  
# --name：设置输出文件名  
```  

**macOS/Linux注意**：如需打包，使用相同命令，文件路径中的分隔符可能需要将 **;** 改为 **:** 


## 🖥 界面概览  
![中文界面](https://github.com/add-qwq/Code-Inserter/blob/main/Code-Inserter-CN.png?raw=true)  
*(通过界面中的**"Switch to English"**按钮切换英文界面。)*  


## 📘 使用指南  

### 步骤1：输入网站ID  
1. 在标有**"网站ID"**的文本区域中，输入Umami的**data-website-id**值（每行一个）  
   - 示例：  
     ```  
     你的网站ID-1  
     你的网站ID-2  
     ```  

### 步骤2：选择文件  
1. 点击**"选择文件"**按钮，从本地目录选择HTML/.htm/.php文件  
2. 使用**"移除选中文件"**或**"清空文件列表"**管理文件队列 

### 步骤3：注入代码  
1. 点击**"一键注入统计代码"**按钮  
2. 确认操作（系统会自动创建备份文件）  
3. 在状态栏和进度条中监控处理进度 

### 操作完成  
- 若所有文件处理成功，将显示成功提示  
- 若部分文件失败，可在状态栏查看详细信息  


## 📜 许可证  
本项目采用 [Apache 2.0 许可证](https://github.com/add-qwq/Code-Inserter/blob/main/LICENSE)


## 🙋 反馈与贡献  
- **问题反馈**：在 [Issues 页面](https://github.com/add-qwq/Code-Inserter/issues) 提交bug或功能请求 
- **代码贡献**：Fork仓库并提交Pull Request
