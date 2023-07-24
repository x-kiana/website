---
title: "Poem #1"
date: 2022-04-23T19:27:14-07:00
draft: false 
---
{{< figure src="forget-me-not.png" width="320vw" height="400vh" >}}
Sometimes the flowers come with poems, so let's have a bit of fun with it.
To read the poem, copy the code below to a .c file and compile it.
Run it, and when prompted paste the content of this file into the terminal:
[forget-me-not](/forget-me-not.txt)

```
 #include <stdio.h>
  #include <stdlib.h>

  #define POEM_SIZE 413

  int main() {
    char* poem = malloc(sizeof(char));
    int x = 1;
    printf("paste what you copied on the website :) ");
    for (int i = 0; i < POEM_SIZE; i++) {
      scanf("%2x", &x);
      poem[i] = (char)x;
      if (x == 0) {
        break;
      }
    }
    printf("\n%s\n", poem);
    free(poem);
    return 0;
  } 
```

