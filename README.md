# mip-api-site

MIP API 接口

## 声明

非官方，只是个人玩玩。

## 接口列表

- [获取组件信息 - /api/components](#components)
- [验证 MIP-JS 代码规范 - /api/validate/js](#js)
- [验证 MIP-HTML 代码规范 - /api/validate/mip](#mip)
- [验证组件 README.md 格式规范 - /api/validate/readme](#readme)
- [HTML 代码转 MIP-HTML 代码 - /api/html2mip](#html2mip)
- [MIP-HTML 代码转 MIP-Cache 代码 - /api/mip2cache](#mip2cache)

### 通用约定

- 支持 CORS 跨域或者 JSONP
- 统一以 JSON 格式返回
- 统一返回结构：

```json
{
    "status": 0,
    "data": {}
}
```

<a id="components"></a>
### 获取组件信息

#### 链接

/api/components

#### 请求类型

GET

#### 返回值

```json
{
    "status": 0,
    "data": [
        {
            "type": "core",
            "name": "mip-iframe",
            "version": "1.0.1",
            "url": null,
            "deps": []
        },
        {
            "type": "extensions",
            "name": "mip-list",
            "version": "1.0.2",
            "url": "https://c.mipcdn.com/static/v1/mip-fixed/mip-list.js",
            "deps": [
                "https://c.mipcdn.com/static/v1/mip-fixed/mip-fixed.js"
            ]
        },
        {
            "type": "platform",
            "name": "mip-mipengine-preview",
            "version": "1.0.2",
            "url": "https://c.mipcdn.com/static/v1/mip-mipengine-preview/mip-mipengine-preview.js",
            "deps": []
        }
    ]
}
```

<a id="js"></a>
### 验证 MIP-JS 代码规范
#### 链接

/api/validate/js

#### 请求参数

参数名 | 说明 | 是否必选
--- | --- | ---
content | 代码内容 | 是

#### 返回值

```json
{
    "status": 0,
    "data": [
    ]
}
```

<a id="mip"></a>
### 验证 MIP-HTML 代码规范
#### 链接

/api/validate/mip

#### 请求参数

参数名 | 说明 | 是否必选
--- | --- | ---
content | 代码内容 | 是

#### 返回值

```json
{
    "status": 0,
    "data": [
    ]
}
```

<a id="readme"></a>
### 验证组件 README.md 格式规范
#### 链接

/api/validate/readme

#### 请求参数

参数名 | 说明 | 是否必选
--- | --- | ---
content | 代码内容 | 是

#### 返回值

```json
{
    "status": 0,
    "data": [
    ]
}
```

<a id="html2mip"></a>
### HTML 代码转 MIP-HTML 代码
#### 链接

/api/html2mip

#### 请求参数

参数名 | 说明 | 是否必选
--- | --- | ---
content | 代码内容 | 是

#### 返回值

```json
{
    "status": 0,
    "data": [
    ]
}
```

<a id="mip2cache"></a>
### MIP-HTML 代码转 MIP-Cache 代码
#### 链接

/api/mip2cache

#### 请求参数

参数名 | 说明 | 是否必选
--- | --- | ---
content | 代码内容 | 是

#### 返回值

```json
{
    "status": 0,
    "data": [
    ]
}
```

