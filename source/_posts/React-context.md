---
title: React context
date: 2021-03-14 22:53:09
tags:
---

# 创建
```typescript
const {Provider,Consumer} = createContext(DefaultValue)
```

* Provider 数据提供方
```typescript
<Provider value={/*共享的数据*/}>
{/*渲染内容*/}
</Provider>
```
* Consumer 数据消费方
```typescript
<Consumer>
{value => /*渲染内容*/}
</Consumer>
</Provider>
```
* 类组件特有方式
```typescript
Class.contextType = Context
// 值由 this.context获取
```
* 函数组件特有方式
```typescript
const value = useContext(Context)
```