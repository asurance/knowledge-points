---
title: react 生命周期
date: 2021-01-27 21:00:27
tags:
---

# hook

* constructor(props)
* componentDidMount()
* componentDidUpdate(prevProps, prevState, snapshot)
* componentWillUnmount()
* shouldComponentUpdate(nextProps, nextState)
* static getDerivedStateFromProps(props, state)
* getSnapshotBeforeUpdate(prevProps, prevState)
* static getDerivedStateFromError(error)
* componentDidCatch(error, info)

# 挂载时

* constructor -> getDerivedStateFromProps -> render -> update DOM tree -> componentDidMount

# 更新时

* new props -> getDerivedStateFromProps -> shouldComponentUpdate -> render -> update DOM tree -> getSnapshotBeforeUpdate -> componetDidUpdate
* setState -> getDerivedStateFromProps -> shouldComponentUpdate -> render -> update DOM tree -> getSnapshotBeforeUpdate -> componetDidUpdate
* forceUpdate -> getDerivedStateFromProps -> render -> update DOM tree -> getSnapshotBeforeUpdate -> componetDidUpdate

# 卸载时

* componetWilUnmount

# 错误时
* componentDidCatch -> setState正常流程