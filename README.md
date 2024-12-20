# 简介

`Bricks` 旨在将爬虫开发变得像搭建积木一样简单而有趣。这个框架的核心理念是提供一个直观、高效的方式来构建复杂的网络爬虫，同时保持代码的简洁和可维护性。无论您是刚入门的新手还是经验丰富的专家，`Bricks` 都能让您轻松地搭建起强大的爬虫，满足从简单数据抓取到复杂网络爬取的各种需求。

通过精心设计的接口和模块化的结构，`Bricks` 使得组合、扩展和维护爬虫变得前所未有的容易。您可以像搭积木一样，快速组合出适合您需求的爬虫结构，无需深入底层细节，同时也能享受到定制化和控制的乐趣。使用 `Bricks`，您将体验到无与伦比的开发效率和灵活性，让爬虫开发不再是一件费时费力的任务。


# 特性

`Bricks` 拥有以下特性

- 基于事件触发拓展爬虫，在定义好自己爬虫主体逻辑的情况下，可以在不修改核心代码的情况下，在请求前后，存储前后等多个事件接口进行拓展，让爬虫流程更加清晰
- 多个爬虫基类，可以有纯代码是的 `air` 爬虫，还有流程化自定义的配置式 `form` 爬虫，还有固定流程的配置式 `template` 爬虫
- 丰富的解析器，包括 `json` / `xpath` / `jsonpath` / `regex` / `json` / 自定义，并且支持配置式书写解析规则
- 灵活可拓展的下载器，目前内置的下载器为 `curl-cffi` ，并且还有可选的 `requests` /  `requests-go` / `pycurl` / `Playwright`， 开发者可以根据规范自己定制下载器
- 灵活的调度器，调度器支持处理同步任务和异步任务，并且支持根据当前任务数量自动调节 `Worker` 数量
- 内置 `Local` 和 `Redis` 两种任务队列，以便应用单机和分布式爬虫


# 安装
## 安装最新代码
```
pip install -U git+https://github.com/KKKKKKKEM/bricks.git
```

## 安装正式版
```
pip install -U bricks-py
```

## 安装测试版
```python
# beta 版本全部都发布在 test.pypi.org
pip install -i https://test.pypi.org/simple/ -U bricks-py

```

# 使用文档
具体文档请查看 [Bricks Docs](https://kkkkkkkem.vercel.app/bricks)

