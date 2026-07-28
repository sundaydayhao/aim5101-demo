# aim5101-demo

AiM5101 GPIO 示例工程，包含 AiM5101 平台相关的 CSI 驱动、板级初始化、基础库和 GPIO 示例代码。

## 目录结构

- `aim5101.cdkws`：CDK 工作区文件
- `cdkws.mk`：工作区 Makefile 入口
- `doc/`：芯片手册和参考文档
- `gpio/board/`：板级初始化与链接脚本
- `gpio/csi_core/`：CSI Core 头文件
- `gpio/csi_driver/`：AiM5101 驱动实现
- `gpio/libs/`：基础库源码
- `gpio/projects/examples/driver/gpio/`：GPIO 示例工程
- `gpio/utilities/`：调试和烧录辅助脚本

## 构建

可使用 CDK 打开 `aim5101.cdkws`，或根据本地工具链环境通过 Makefile 构建：

```sh
make -f cdkws.mk
```

构建产生的 `Obj/`、`Lst/` 等目录已在 `.gitignore` 中忽略。
