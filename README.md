## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run dev
```

### Compiles and minifies for production
```
npm run build
```

使用方法：
1. 配置根目录下vue.init -> route -> config.js 
    <br />
    views: 路由所在文件夹
    <br />
    excludes：该文件不自动生成路由
    <br />
    custom：自定义路由
    <br />
    output：输出结果所在文件
    <br />
    src/views/test/view4/_id.vue会生成以下路由：
    ```
    {
		"path": "/test/view4/:id?",
		"name": "TestView4",
		"component": "test/view4/_id.vue"
	}
    ```
    如果id参数需要必选，可以在_id文件夹下创建index.vue
    <br />
2. 配置根目录下vue.init -> lang -> config.js 
    <br />
    cn: 简体语言文件路径
    <br />
    tw：需要自动生成繁体的文件路径
    <br />
    type：多语言keys类型文件路径(.d.ts)
    <br />
3. 使用``` node vue.init ```自动生成路由及繁体翻译
    <br />
4. 使用``` npm run dev ```启动项目
    <br />
5. 配置src -> router -> meta.json
    <br />
    auth： 权限
    <br />
    keepalive： 路由是否缓存
    <br />
    multiple： 相同路由是否可开启多个
    <br />
5. 配置src -> router -> menus.json，生成菜单
    <br />
    name： 目标路由name，用于跳转
    <br />
    icon： 菜单图标
    <br />
    title： 菜单名(多语言key)
