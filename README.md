# xiaojiqiao
Small techniques that better to be memorized

# 1. 烦人的端口被占用? Port 3000 is already in use 杀掉它
  step1: 
  ```
  $ lsof -i tcp:3000
  ```
  在return一堆东西 找到一种的 PID (process identifier)
  
  step2: 
  ```
  $ kill -9 `${the PID found in step1}` 
  ```
