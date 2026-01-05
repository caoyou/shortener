# shortener
短链服务。工程训练项目；Clean Architecture 极简版。

# 架构图
shortener/
├── api/
│   └── routes.py        # 路由层（只放 HTTP 逻辑）
├── domain/
│   └── models.py        # 纯 Python 类，定义 Link 实体
├── repository/
│   └── link_repo.py     # 数据访问（SQLite 增删查）
├── service/
│   └── shortener.py     # 核心业务逻辑（如何生成短码、如何查）
├── tests/
│   └── test_shortener.py # 单元测试
├── config.py            # 配置集中管理
├── database.py          # SQLite 连接会话
├── main.py              # FastAPI 启动入口
├── Dockerfile           # 写 Dockerfile + docker-compose.yml，本地一键启动
├── README.md            # 用 Markdown 画一张架构图
└── requirements.txt     

Day1: 项目骨架 + 架构图 ✅
