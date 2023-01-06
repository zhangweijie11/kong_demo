### 操作步骤

1. 执行 prepare.sh 文件，生成kong 和 konga 数据库，随后自动执行数据库迁移操作
2. kong 容器挂载自定义插件，注意修改 constants.lua 文件中的 plugins 参数（可选操作，如果没有自定义插件可跳过）
3. 执行 docker-compose up 启动 kong、konga、pg 三个容器