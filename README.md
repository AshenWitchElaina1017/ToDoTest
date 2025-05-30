## ✨ 萌萌哒待办清单 ✨

这是一个基于Flask框架开发的动漫风格待办清单应用，集成了MySQL数据库进行数据持久化。它不仅提供了基本的待办事项管理功能，还通过精心设计的UI和动画效果，为用户带来了愉悦的视觉体验。

### 功能特性

- **动漫风格UI**：界面设计充满动漫元素，包括可爱的角色头像、背景装饰和动画效果。
- **CRUD操作**：支持待办事项的创建（Create）、读取（Read）、更新（Update，标记完成/未完成）和删除（Delete）功能。
- **数据持久化**：所有待办事项数据都存储在MySQL数据库中，确保数据不会丢失。
- **任务筛选**：提供“全部”、“已完成”和“待处理”三种筛选模式，方便用户快速查看不同状态的任务。
- **实时统计**：实时显示任务总数、已完成任务数和待处理任务数。
- **交互动画**：添加、完成或删除任务时，伴随有火花、庆祝和漂浮图标等动画效果，增强用户体验。
- **响应式设计**：界面在不同设备上均能良好显示。
- **消息提示**：通过Toast通知提供操作反馈。

### 技术栈

- **后端**：
  - Python 3
  - Flask (Web框架)
  - Flask-MySQLdb (MySQL数据库连接)
- **前端**：
  - HTML5
  - CSS3 (包括Flexbox布局、动画、响应式设计)
  - JavaScript (原生JS，实现前端逻辑和动画)
  - Font Awesome (图标库)
  - Google Fonts (中文字体)
- **数据库**：
  - MySQL

### 安装与运行

请按照以下步骤在本地环境中设置和运行项目：

#### 1. 克隆仓库

```bash
git clone https://github.com/AshenWitchElaina1017/ToDoTest
cd ToDoDemo
```

#### 2. 创建Python虚拟环境（推荐）

```bash
python -m venv venv
venv\Scripts\activate  # Windows
# source venv/bin/activate  # macOS/Linux
```

#### 3. 安装依赖

```bash
pip install -r requirements.txt
```

#### 4. 配置MySQL数据库

确保您的系统上安装并运行了MySQL数据库。本应用默认使用`root`用户和密码`1017`连接数据库。如果您使用不同的凭据，请修改 `app.py` 中的数据库配置。

应用启动时会自动创建名为 `todo_db` 的数据库和 `todos` 表（如果它们不存在）。

您也可以手动创建数据库：

```bash
mysql -u root -p -e "CREATE DATABASE IF NOT EXISTS todo_db;"
```

#### 5. 运行应用

```bash
python app.py
```

应用将在 `http://127.0.0.1:5000` 启动。您可以在浏览器中访问此地址来使用待办清单。

### 项目结构

```
ToDoDemo/
├── app.py              # Flask后端应用逻辑
├── requirements.txt    # Python依赖列表
├── static/
│   ├── css/
│   │   └── style.css   # 动漫风格UI样式
│   ├── images/         # 动漫角色图片和背景装饰
│   │   ├── 01.jpeg
│   │   ├── ...
│   │   └── icon.ico
│   └── js/
│       └── script.js   # 前端交互逻辑和动画效果
└── templates/
    └── index.html      # 应用主页面HTML结构
```

### 未来增强

- **用户认证**：添加用户注册和登录功能，实现多用户待办清单。
- **任务优先级**：允许用户设置任务的优先级。
- **截止日期**：为任务添加截止日期功能。
- **通知提醒**：集成桌面通知或邮件提醒功能。
- **更多动漫元素**：引入更多动漫角色、主题和音效。
- **拖拽排序**：允许用户通过拖拽来调整任务顺序。
- **搜索功能**：添加任务搜索功能。

希望这个README文档能帮助您更好地了解和使用这个项目！
