#!/bin/python3

import math
import os
import random
import re
import sys

#
# Complete the 'jumpingOnClouds' function below.
#
# The function is expected to return an INTEGER.
# The function accepts INTEGER_ARRAY c as parameter.
#

def jumpingOnClouds(c):

    jumps = 0
    idx = 0
    while (idx < len(c)):
        if idx+1 < len(c) and c[idx+1] == 0:
            if idx+2 < len(c) and c[idx+2] == 0:
                idx += 2
            else:
                idx += 1
        else:
            idx += 2
        jumps += 1
        
    return jumps-1

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    n = int(input().strip())

    c = list(map(int, input().rstrip().split()))

    result = jumpingOnClouds(c)

    fptr.write(str(result) + '\n')

    fptr.close()
