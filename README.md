# PyHero
A ~~terrible~~ great Guitar Hero III clone made in PyGame

This was a project I did for the final for my Advanced Computer Programming class at school (almsot a year ago at the time the creation of this repo). We were tasked with making a video game in PyGame. Those were really the only guidelines, as long as the teacher believed we could get it done in time.

Some features include:
* The ability to load almost any chart from GH3, albeit with modifications required
* Controller support (only tested with XBox 360 Xplorer guitar)
* Those are the only two features that are even semi-remarkable

If you want to check it out, I *highly* suggest watching [this video](https://www.youtube.com/watch?v=MeYfBIGKki8) instead of trying to run it yourself. I have ONLY tested it on Python 2.7, with the PyGame build included in the dependencies folder. You also need to put `pygbutton.py` (also in the dependencies folder) in the same folder as `PyHero.py`. If you're really desperate for some free guitar hero action, I'd recommend checking out [Clone Hero](https://www.youtube.com/channel/UCc3IfdqGZjhdgQbi_EpfuYg) instead.

I don't intend to ever work on or update this project again. I made some mistakes early on when creating this that would essentially require me to rewrite most of the program if I wanted to develop it further. These include:
* All the calculations I do are framerate-dependent, while the audio continues to play at the same rate regardless of framerate. This means that audio is practically guaranteed to desync if the chart that you are playing is not fiddled with extensively, and the changes needed (namely to the `divisor` value) will vary from computer to computer. 
* I did not fully understand how chart Guitar Hero calculates note positions based on info in the charts. Namely, I decided to try and ignore tempo, which was a very bad idea. Any song with a tempo change will end up desyncing from the audio 100% of the time, and there is nothing you can do about it.
*Probably more that I can't think of

Despite all its shortcomings, I'm rather proud of what I was able to accomplish. PyGame (and Python in general) don't seem to be built for this type of thing. If I were to revisit this, I would probably scrap everything here and do it in Unity instead, but working on this for a month and a half kind of ruined my desire to ever perfect this. I'd rather move on to other things.
