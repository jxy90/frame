# frame
- go backend frame
  - cobra + grpc-gateway + gorm + redis + viper + swagger +zap




```cgo
project/
├── cmd/                 # 应用程序入口
│   ├── app/             # 主应用程序
│   └── migrate/         # 数据迁移脚本
├── config/              # 配置文件和配置加载
├── internal/            # 私有应用逻辑（Go Modules 推荐）
│   ├── app/             # 各个服务的核心业务逻辑
│   │   ├── handler/     # HTTP/GRPC 的处理器
│   │   ├── service/     # 服务层（核心业务逻辑）
│   │   ├── repository/  # 数据访问层（DAO 或 Repository）
│   │   ├── model/       # 数据模型（数据库表结构、DTO）
│   │   └── dto/         # 数据传输对象（输入输出结构）
│   └── pkg/             # 可复用模块（工具类、通用逻辑）
├── docs/                # 文档（API 文档、设计文档）
├── pkg/                 # 公共模块（通用库、工具库）
├── scripts/             # 脚本文件（如部署、构建脚本）
├── test/                # 测试文件（集成测试、功能测试）
├── go.mod               # Go Modules 定义
└── main.go              # 主入口文件

```