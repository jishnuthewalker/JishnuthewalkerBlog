The first time I heard of typography, I had just been introduced into design. I was amazed that so much detail and structure goes behind just fonts that we take for granted. Then I would browse through Foundries and Font collections just figuring looking at admiring fonts. to me it was a spectacle. 

Over the year I would always come across the frustration of never being able to smoothly transition from the different weights of fonts. It never made sense to me why it was just so impossible. (I was really dumb) In 2018, I had understood a bit of the technical limitations of why fonts can't animate, I heard about Variable fonts. My mind, was BLOWN 🧠💥. Somehow, designers and engineers came together across the world and built a method of solving this was nothing short of amazing.

I went on to experiment and use variable font wherever I could. Though it was never the focus of my work it always managed to come in clutch every time I was working with type.

![[ANgoor_030001-0060.gif | 500]]

![[Composition 3.gif | 500]]

![[zen_41Wx6oTqQo (2).gif | 500]]


In my DES, I embarked on a journey to figure of a workflow to use Variable font for animation. Explore the existing tools that allow for variable fonts and explore the visuals and outputs of using them.

![[Variable Typography DES.mp4 | 500]]


![[ColdType_V3.mp4]]


![[ColdType_V1.mp4]]


![[ColdType_V2.mp4]]

# Using Coldtype in blender

So there is an addon called [ST2](https://coldtype.xyz/st2/) for blender developed by [Rob Stenson](https://robstenson.com).

but i have no idea how to use it. So i decided to use the [coldtype](https://github.com/coldtype/coldtype) library and set that up instead (Instructions also provided by Rob on the coldtype docs)

Let me get right to it, it was a pain. This wasn't even the first time using the library but it was still really difficult to install. Wrapping my head around [venv](https://docs.python.org/3/library/venv.html) and using coldtype along with [b3denv](https://github.com/coldtype/b3denv) (a tool by Rob to help expose [blender's python api](https://docs.blender.org/api/current/index.html). 

This is just my was of documenting my process and maybe help someone out if they ever get stuck where i did.

So in a nutshell cold type works best in a python Virtual environment or [venv](https://docs.python.org/3/library/venv.html) this is a way to isolate different python versions on a single computer. this help mitigate dependency problems and makes the process much more streamlined.

The way to go about this is

Installing python
- Make sure you have [python](https://www.python.org/downloads/) installed. I am using Python 3.12.8.
- Make sure python is added to system PATH. (Google it, there's lots of guides)
you can check this by typing `python --version` in the terminal.

Activating venv
- navigate to a folder you want to code in
- open it in terminal (you can also navigate to the folder in the terminal by using `cd path/to/folder` replace the "path/to/folder" by the actual path to the folder)
- here you can run `python -m venv venv` this is telling python to make a virtual environment named 'venv'. This will create a venv directory in the folder.
- now you run the command `./venv/Scripts/Activate.ps1` (This command is for windows)
- for MacOS and Linux I think you need `source venv/bin/activate`
- you will see that you have 'venv' written before you directory in the terminal, usually in green, indicating that you are in the virtual environment. 

Installing Coldtype(not b3d version)
- now here you can run the command `pip install "coldtype[viewer]"` 
- to test if installed properly you can run `coldtype demo`
- to run a file or make a new one use `coldtype path/to/file.py`

Installing Coldtype(with b3d)
- make sure you have blender installed (It's so much easier if you have it installed in the default location, you'll save yourself so much hassle, if not refer to this part of the [readme](https://github.com/coldtype/b3denv?tab=readme-ov-file#non-default-blender-installs) )
- here you can run `b3denv python -m venv benv`. This will setup a virtual environment named 'benv'
- Now, to activate the environment run `./venv/Scripts/Activate.ps1` 
- I had to install cold type again by `coldtype demo` 
- make sure the python file includes the headers,

```
from coldtype.blender import *

from coldtype import *
```

- now you should be able to test the install by `coldtype examples/blender/varfont.py -p b3d`
- -p is a flag for property I think and b3d is to set it up for blender
- alternatively you can use `coldtype examples/blender/varfont.py -bw 1` but I have not tested this yet. 
