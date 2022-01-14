
#### 模块创建流程

1. 新建一个文件夹以模块名字命名 例如 LIMBase
2. 进入 LIMBase 执行 yarn init -y  将得到package.json文件，修改里面的 name字段为 limbase (因为node项目规定项目名字只能为小写)
3. 执行 tsc --init 将获得tsconfig.json文件（如果没有tsc命令 执行 sudo npm install -g typescript）
4. 将tsconfig.json里的 declaration: true 和  outDir:"./lib" 打开 (declaration为true表示生成 `.d.ts` 文件 outDir表示生成文件的目录)