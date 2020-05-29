---
layout: post
title: python基础练习
date: 2020-05-29
categories: blog
tags: [python,while]
description: continue。
---

公司的小朋友在学习python，做while循环和if条件判断的练习，结果给我也绕蒙了。看来还是基础不扎实。
### 记录下来：
```
# -*- coding:UTF-8 -*-
#! python3

age = 25
counter = 0

while counter < 3:
    inAge = int(input('Please enter your guessed age: \n'))
    if inAge == age:
        print('Awesome! Your guessed right!')
        break
    elif inAge < age:
        print('Guess the age is young!')
    elif inAge > age:
        print('Guess the older age!')

    counter += 1

    if counter >= 3:
        print('If you enter Y or y, the game will continue. \n \
            If you enter N or n, you will exit the game. \n')
        cho = input('Please make your choice： \n')

        if cho == 'Y' or cho == 'y':
            print('The game continues！')
            counter = 0
            continue
        else:
            print('The game exit!')
            break
```
