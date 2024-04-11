# xrem
I have bad anxiety and other issues which affects my memory so when i want to remember what i did the day before on my pc. i use this setup as i wanted something simple. It has less features than offical repo but could help someone else too... :



ffmpeg -f gdigrab -framerate 2 -i desktop -vf "drawtext=fontfile=./FiraCode-Light.ttf: text='%{localtime}': x=10: y=10: fontsize=24: fontcolor=white: box=1: boxcolor=black@0.5" output.mkv  -preset ultrafast

https://trac.ffmpeg.org/wiki/Capture/Desktop

only uses 0.1 cpu.

plus c++ software that keeps track of windows titles, clipboard 
