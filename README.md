# xrem
I have bad anxiety and other issues which affects my memory so when i want to remember what i did the day before on my pc. i use this setup as i wanted something simple. It has less features than offical repo but could help someone else too... :



ffmpeg -f gdigrab -framerate 2 -i desktop -vf "drawtext=fontfile=c\\:/windows/fonts/arial.ttf: text='%{localtime}': x=10: y=10: fontsize=24: fontcolor=white: box=1: boxcolor=black@0.5" output.mkv -preset ultrafastg

ffmpeg -f gdigrab -framerate 2 -i desktop -c:v libx265 -crf 30 -vf "drawtext=fontfile=c\:/windows/fonts/arial.ttf: text='%{localtime}': x=10: y=10: fontsize=24: fontcolor=white: box=1: boxcolor=black@0.5" output.mkv -preset ultrafast
high cpu but low disk

https://trac.ffmpeg.org/wiki/Capture/Desktop

only uses 1 - 4 cpu.



ffmpeg -framerate 3 -f x11grab -i :0.0 output.mp4 -preset ultrafast
