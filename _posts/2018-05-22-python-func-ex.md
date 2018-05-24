---
layout: post
title:  "[Python 03함수] - 함수실습"
subtitle:   "함수실습"
categories: language
tags: python
comments: true
---


##### 1. 매개변수로 문자열을 받고, 해당 문자열이 red면 apple을, yellow면 banana를, green이면 melon을, 어떤 경우도 아닐 경우 I don't know를 리턴하는 함수를 정의하고, 사용하여 result변수에 결과를 할당하고 print해본다.
```
>>> def output_fruits():
      colors = input()
      if colors == 'red':
          result = 'apple'
      elif colors == 'yellow':
          result = 'banana'
      elif colors == 'green':
          result = 'melon'
      else:
          result = 'I don\'t know'
      return result
>>> output_fruits()
green

'melon'
```

##### 2. 1번에서 작성한 함수에 docstring을 작성하여 함수에 대한 설명을 달아보고, help(함수명)으로 해당 설명을 출력해본다.
```
def output_fruits():
    'input color then print fruit name'
    colors = input()
    if colors == 'red':
        result = 'apple'
    elif colors == 'yellow':
        result = 'banana'
    elif colors == 'green':
        result = 'melon'
    else:
        result = 'I don\'t know'
    return result

help(output_fruits)

```

##### 3. 한 개 또는 두 개의 숫자 인자를 전달받아, 하나가 오면 제곱, 두개를 받으면 두 수의 곱을 반환해주는 함수를 정의하고 사용해본다.
```
def multi_or_square(*args):
    if len(args) == 1:
        result = args[0]**2
    else:
        result = args[0]*args[1]
    return result
```


##### 4. 두 개의 숫자를 인자로 받아 합과 차를 튜플을 이용해 동시에 반환하는 함수를 정의하고 사용해본다.
```

```


##### 5. 위치인자 묶음을 매개변수로 가지며, 위치인자가 몇 개 전달되었는지를 print하고 개수를 리턴해주는 함수를 정의하고 사용해본다.
```
```

##### 6. 람다함수와 리스트 컴프리헨션을 사용해 한 줄로 구구단의 결과를 갖는 리스트를 생성해본다.
```
```
