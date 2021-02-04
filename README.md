# mono-project

```shell

# 添加子项目依赖项到 package.json, 只能单个添加
yarn run add <package>[@version] [--dev] [--exact] [--peer]

# create 是创建子项目命令，loc 为目标路径, 目录不存在时需要优先创建
yarn run create package-name <loc>

# 执行 symlink 操作，符合语义化版本号的会 link 到本地文件，否则通过远程安装
yarn run bootstrap

# 列出所有的依赖包
yarn run list

# 执行每个子项目的测试用例
yarn run test

# 清空根目录及子项目下的所有 node_modules（如果你进入submodule内安装了submodule的依赖，则可能项目依赖引用会出错，请先执行此命令清除node_modules后，再到monorepo根目录执行`yarn install`）
yarn run clean

# 子项目下的构建出来的文件 (依赖子项目的 clean 命令)(如果发现submodule 下引用了monorepot下相关modules下的dist下的文件，请先删除dist `yarn run clean:build`)
yarn run clean:build

```
