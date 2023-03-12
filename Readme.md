# 15 Patterns using Python

![Python Pattern](pattern-image.jpg)

### Pattern #1

```
pattern_size = int(input("Pattern Size: "))
for _ in range(pattern_size):
    print("*" * pattern_size)

Output:
*****
*****
*****
*****
*****
```

### Pattern #2

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size + 1):
    print("*" * i)

Output:
*
**
***
****
*****
```

### Pattern #3

```
pattern_size = int(input("Pattern Size: "))
for i in range(pattern_size, 0, -1):
    print("*" * i)

Output:
*****
****
***
**
*
```

### Pattern #4

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size + 1):
    for j in range(1, i + 1):
        print(j, end=" ")
    print("\r")

Output:
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```

### Pattern #5

```
pattern_size = int(input("Pattern Size(Odd number only > 5): "))
for i in range(1, pattern_size + 1):
    print("*" * i)
for j in range(pattern_size - 1, 0, -1):
    print("*" * j)

Output:
*
**
***
****
*****
****
***
**
*
```

### Pattern #6

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size + 1):
    spaces = " " * (pattern_size - i)
    stars = "*" * i
    print(f"{spaces}{stars}")

Output:
    *
   **
  ***
 ****
*****
```

### Pattern #7

```
pattern_size = int(input("Pattern Size: "))
for i in range(pattern_size, 0, -1):
    spaces = " " * (pattern_size - i)
    stars = "*" * i
    print(f"{spaces}{stars}")

Output:
*****
 ****
  ***
   **
    *
```

### Pattern #8

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size + 1):
    spaces = " " * (pattern_size - i)
    stars = ("*" * i) + ("*" * (i - 1))
    print(f"{spaces}{stars}")

Output:
    *
   ***
  *****
 *******
*********
```

### Pattern #9

```
pattern_size = int(input("Pattern Size: "))
for i in range(pattern_size, 0, -1):
    spaces = " " * (pattern_size - i)
    stars = ("*" * i) + ("*" * (i - 1))
    print(f"{spaces}{stars}")
Output:
*********
 *******
  *****
   ***
    *
```

### Pattern #10

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size + 1):
    spaces = " " * (pattern_size - i)
    stars = "* " * i
    print(f"{spaces}{stars}")

Output:
    *
   * *
  * * *
 * * * *
* * * * *
```

### Pattern #11

```
pattern_size = int(input("Pattern Size: "))
for i in range(pattern_size, 0, -1):
    spaces = " " * (pattern_size - i)
    stars = "* " * i
    print(f"{spaces}{stars}")

Output:
* * * * *
 * * * *
  * * *
   * *
    *
```

### Pattern #12

```
pattern_size = int(input("Pattern Size: "))
for i in range(pattern_size, 0, -1):
    spaces = " " * (pattern_size - i)
    stars = ("* " * i)
    print(f"{spaces}{stars}")

for j in range(1, pattern_size + 1):
    spaces = " " * (pattern_size - j)
    stars = "* " * j
    print(f"{spaces}{stars}")
Output:
* * * * *
 * * * *
  * * *
   * *
    *
    *
   * *
  * * *
 * * * *
* * * * *
```

### Pattern #13

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size + 1):
    spaces = " " * (pattern_size - i)
    stars = "* " * i
    if  i >= 3 and i < pattern_size:
        mid_spaces = len(stars) - 3
        stars = "*" + (" " * mid_spaces) + "*"
    elif i == pattern_size:
        stars = ("*" * i) + ("*" * (i - 1))

    print(f"{spaces}{stars}")
Output:
    *
   * *
  *   *
 *     *
*********
```

### Pattern #14

```
pattern_size = int(input("Pattern Size: "))
for i in range(pattern_size, 0, -1):
    spaces = " " * (pattern_size - i)
    stars = "* " * i
    if  i >= 3 and i < pattern_size:
        mid_spaces = len(stars[1:-1]) - 1
        stars = "*" + (" " * mid_spaces) + "*"
    elif i == pattern_size:
        stars = ("*" * i) + ("*" * (i - 1))

    print(f"{spaces}{stars}")
Output:
*********
 *     *
  *   *
   * *
    *
```

### Pattern #15

```
pattern_size = int(input("Pattern Size: "))
for i in range(1, pattern_size):
    spaces = " " * (pattern_size - i)
    stars = "* " * i
    if  i >= 3 and i < pattern_size:
        mid_spaces = len(stars[1:-1]) - 1
        stars = "*" + (" " * mid_spaces) + "*"

    print(f"{spaces}{stars}")

for j in range(pattern_size, 0, -1):
    spaces = " " * (pattern_size - j)
    stars = "* " * j
    if  j >= 3 and j <= pattern_size:
        mid_spaces = len(stars[1:-1]) - 1
        stars = "*" + (" " * mid_spaces) + "*"

    print(f"{spaces}{stars}")


Output:
    *
   * *
  *   *
 *     *
*       *
 *     *
  *   *
   * *
    *
```

## **[Connect with me]()**

<p align="left">
    <a href="#">
        <img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube"/>
    </a>
    <a href="https://twitter.com/ashishjaiswar_">
        <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"/>
    </a>
    <a href="https://www.linkedin.com/in/ashish-jaiswar-developer/">
        <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
    </a>
    <a href="mailto:ashish.jaiswar687@gmail.com">
        <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/>
    </a>
    <a href="https://medium.com/@ashishjaiswar">
        <img src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" alt="Medium"/>
    </a>
    <a href="https://github.com/AshishJaiswar">
        <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github"/>
    </a>

</p>

## **[You can always buy me a coffee]()**

<a href="https://www.buymeacoffee.com/AshishJaiswar">
        <img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" alt="Byemecoffee"/>
    </a>

#### Enjoy Coding ❤
