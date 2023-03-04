import re

"""**************************************************************************"""
# 1


def to_camel_case(text):
    return re.split('_|-', text)[0] + ''.join(word.title() for word in re.split('_|-', text)[1::])


print(to_camel_case('some_word-wooohooo'))

"""**************************************************************************"""
# 2


class SingletonMeta(type):

    _instances = {}

    def __call__(cls, *args, **kwargs):
        if cls not in cls._instances:
            cls._instances[cls] = super(SingletonMeta, cls).__call__(*args, **kwargs)
        return cls._instances[cls]


"""**************************************************************************"""
# 3
n = 5
count_bits = bin(n).count('1')
print(count_bits)


"""**************************************************************************"""
# 4


def digital_root(n):
    return n if n < 10 else digital_root(sum(map(int, str(n))))


"""**************************************************************************"""
# 5


n = 5
even_or_odd = lambda number: "Even" if number % 2 == 0 else "Odd"
print(even_or_odd(n))
