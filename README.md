# Complex API.py
This the source code for the python module I have built/working on.

This module makes it easy to use my [API](https://github.com/JagTheFriend/APICode)

Currently, the API supports:
  + compiling the code(of different languages) and getting the output
  + getting a random post from a _subreddit_
  + getting the lyrics of a song

  + generating pixel art
  + getting the weather of a place
  + finding the length of a youtube playlist

  + getting a random inspirational text
  + getting a result of a calculation
  + converting hexadecimal to decimal(or denary)
  + converting decimal(or denary) to binary


# Code snippets
In order to use the API,
you need to first download [this module (`pip install Complex-API`)](https://pypi.org/project/Complex-API/)

## Compile API:
[Example:](https://github.com/JagTheFriend/Complex-API/pulls)
```py
from Complex_API import complex_api
# run python
lang = "python"
code = '''
print('hello')
'''
print(complex_api.compile(lang=lang, code=code))
# run java
lang = "java"
code = '''
class Compiler{
    public static void main(String[] args){
        System.out.println("This works");
    }
}
'''
print(complex_api.compile(lang=lang, code=code))
```
[Get all the supported languages here](https://API.jagthefriend.repl.co/compile=support_support)

## Reddit API:
[Example:](https://API.jagthefriend.repl.co/reddit=meme+10)
```py
from Complex_API import complex_api
# example: name_of_subreddit = "meme"
name_of_subreddit = "name_of_a_valid_subreddit"
number_of_posts = 10 # number of posts to be returned
print(complex_api.reddit(limit=number_of_posts, subreddit=name_of_subreddit))
```

## Lyrics API:
[Example:](https://API.jagthefriend.repl.co/lyrics+falling)
```py
from Complex_API import complex_api
SongName = "name of song"
print(complex_api.lyrics(song=SongName))
```

## Pixel Art:
[Example:](https://API.jagthefriend.repl.co/ascii_hello)
```py
from Complex_API import complex_api
text = "Hello gammer"
print(complex_api.ascii(text=text))
```

## Weather API:
[Example:](https://API.jagthefriend.repl.co/temp=America+metric)
```py
from Complex_API import complex_api
# example: place = Cape Town
place = "name of a place"
unit = "metric" # or imperial
print(complex_api.temp(place=place, unit=unit))
```

## Youtube Playlist length finder:
[Example:](https://API.jagthefriend.repl.co/length+PL59LTecnGM1OGgddJzY-0r8vdqibi3S2H)
```py
from Complex_API import complex_api
# example URL: https://www.youtube.com/playlist?list=PL59LTecnGM1OGgddJzY-0r8vdqibi3S2H
# id = PL59LTecnGM1OGgddJzY-0r8vdqibi3S2H
play_list_link = "id"
print(complex_api.length(playlist=play_list_link))
```

## Calculator:
[Example:](https://API.jagthefriend.repl.co/cal_6*9+6+9)
```py
from Complex_API import complex_api
formula = "6*9+6+9"
print(complex_api.calculator(formula=formula))
```

## Inspire API:
[Example:](https://API.jagthefriend.repl.co/inspire)
```py
from Complex_API import complex_api
print(complex_api.inspire())
```

## Hexadecimal to Decimal(or Denary) converter:
[Example:](https://API.jagthefriend.repl.co/hex+ABCDEF)
```py
from Complex_API import complex_api
formula = "A6B9C1D1E1"
print(complex_api.hex_to_denary(hex_code=formula))
```

## Decimal(or Denary) to Binary converter:
[Example:](https://API.jagthefriend.repl.co/binary=1969)
```py
from Complex_API import complex_api
formula = "45713" # any number
print(complex_api.binary_to_denary(binary=formula))
```

## Talk to my chatbot:
[Example:](https://API.jagthefriend.repl.co/ai_"Hello")
```py
from Complex_API import complex_api
text = "Hi" # any text
print(complex_api.ai(text=text))
```

If you find any bugs _or have new ideas_,

Feel free to raise a <br>
[new issue](https://github.com/JagTheFriend/Complex-API/issues)
<br>
Or a <br>
[pull request](https://github.com/JagTheFriend/Complex-API/pulls)
