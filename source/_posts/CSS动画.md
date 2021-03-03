---
title: CSS动画
date: 2021-03-03 22:28:46
tags:
---
# transition
* transition-property 属性
* transition-duration 持续时间
* transition-timing-function 插值函数
* transition-delay 开始动画延迟
* TransitionEvent(存在兼容性问题)
  * transitionrun
  * transitionstart
  * transitioncancel
  * transitionend

# animation
* @keyframes 指定关键帧
* animation-duration 持续时间
* animation-timing-function 插值函数
* animation-delay 延迟
* animation-iteration-count 播放次数
* animation-direction 动画播放方向
  * normal
  * alternate
  * reverse
* animation-fill-mode 结束后的状态
  * none 回到动画开始前
  * backwards 回到动画第一帧
  * forwards 停在最后一帧
  * both 根据animation-direction有forwards或backwords效果
* animation-play-state 播放状态
  * running
  * pause
* animation-name 对应@keyframe
* AnimationEvent(存在兼容性问题)

# step