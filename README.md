# test.py
def proc1(p):
    p[0]=p[1]


def proc2(p):
    p=p+[1]


def proc3(p):
    q=p
    p.append(3)
    q.pop()


def proc4(p):
    q=[]
    while p:
        q.append(p.pop())
    while q:
        p.append(q.pop())


def test1():
    p=[1, 2, 3, 4, 5]
    proc1(p)
    if p == [1, 2, 3, 4, 5]:
        print(True)
    else:
        print(False)


def test2():
    p=[1, 2, 3, 4, 5]
    proc2(p)
    if p == [1, 2, 3, 4, 5]:
        print(True)
    else:
        print(False)


def test3():
    p=[1, 2, 3, 4, 5]
    proc3(p)
    if p == [1, 2, 3, 4, 5]:
        print(True)
    else:
        print(False)

def test4():
    p=[1, 2, 3, 4, 5]
    proc4(p)
    if p == [1, 2, 3, 4, 5]:
        print(True)
    else:
        print(False)





test1()
test2()
test3()
test4()
