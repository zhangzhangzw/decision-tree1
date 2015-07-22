# decision-tree1
My  repository on GitHub2
from numpy import *
from math import log



def inbound(items, store):
    for item in items:
        if item in store:
            store[item] += 1
        else:
            store[item] = 1

goods = ['iPhone', 'kindle', 'kindle', 'newb','new2','new3']


fc = {}

inbound(goods, fc)

print fc
print len(fc)


def outbound(sells, store):
    totalEntropy = 0
    for item in store:
        prob = float(store[item]) / len(sells)
        entropy = - prob * log(prob, 2)
        print item, prob, entropy
        totalEntropy += entropy
    return totalEntropy


print outbound(goods, fc)


value = inf

valueB = 100000000000000

if valueB > value:
    print "bigger"
else:
    print "smaller"


