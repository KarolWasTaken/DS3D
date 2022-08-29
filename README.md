[![pypresence](https://img.shields.io/badge/using-pypresence-00bb88.svg?style=for-the-badge&logo=discord&logoWidth=20)](https://github.com/qwertyquerty/pypresence)

## Due to the newest Dark Souls III update, this program no longer works. It can only be used by manually inputting the data in. If I can, I will implement a fix. 

# DS3D
So one day I decided to make a program called [DS3C](https://github.com/TohruTheMaid/DS3C).
I posted this program to a [Dark souls challenge run community](https://discord.gg/vESQQvm) and they told me that [Team Hitless](https://discord.gg/4E7cSK7) (hitless gamerun community)
has been looking for something just like this but for hits. I thought, "hey why not try and make a hit counter." Now I'm here. Hello :). There are a few issues with how the counter works which I'll expain
in the following sections - aswell as the good parts.
# The Good
The way I see if the player is hit is I get the initial health value and check it against changes every 0.01 seconds.
The counter doesnt increase when the damage done is bellow 7 (to avoid poison counting as hits).
 It also doesnt register healing as a hit which is also nice. This function can be viewed in DarkSoulsDeathCount.py at 
 lines 80 - 102. 
# The Bad
Stuff like fall damage still counts as a hit. Also when the enemy falls on you, thats not counted
as a hit (though it is one). I guess its such a rare occurrence that I shouldnt need to overcomplicate the program for it.
Maybe someone who is better at DS3 modding and python could try and fix this. 
# The Ugly
I am like super lazy so I haven't changed the variable names from 'deaths' to 'hits'.
Everytime something references a death in the code, thats just a hit in disguise. This program is a fork of my own [DS3C](https://github.com/TohruTheMaid/DS3C) program
so they share 99% of the code. I am not a genius programmer so optimisations and general edits to the code 
to make it cleaner are here in plentiful demand. Oh also the console gets spammed up with 'Read Memory - Error Code: 6'. Don't worry thats normal. If you
really want that gone, comment out line 63 in process_interface.py.
## Acknowledgements

 - [Random Davis](https://www.youtube.com/channel/UCEtOy2t4jLY7oNGHfdlMHvA)


## Dependencies
To run the code files, install the following dependencies

- [tkinter](https://tkdocs.com/tutorial/install.html)(preinstalled with python)
- [pywin32](https://pypi.org/project/pywin32/)
- [psutil](https://pypi.org/project/psutil/)
- [pypresence](https://pypi.org/project/pypresence/3.2.0/)


## Authors

- [@TohruTheMaid](https://github.com/TohruTheMaid)

