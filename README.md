# AWESOME

----

####Using RegEx in python:

1. A regex object is created first.
        obj = re.compile(r'[complex regex]')
        data = obj.search([string])
        data.group([_])

        ---- Example ----

        ```re.compile to convert the raw string file to string```
        >>obj = re.compile(r'/d/d/d-/d/d/d-/d/d/d/d')  
        >>num = obj.search('Contact at 123-456-7890')
        >>num.group()
        123-456-7890

    Regex are really important and can have varying complexity. They help to improve pattern searching.

    Python regex are greedy by default. So to use a non-greedy version, use `?` after the `{}`

        ``` This is the greedy version```
        >>obj = re.complile(r'(Ha){,3}')
        >>count = obj.search('HaHaHa')
        >>count.group()
        HaHaHa

        ----

        ```This is the non greedy version```
        >>obj = re.complile(r'(Ha){1,3}?')
        >>count = obj.search('HaHaHa')
        >>count.group()
        Ha
