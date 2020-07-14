# Rofi Nerd Font Cheatsheet
![Picture](https://github.com/groovykiwi/rofi-nerdfont/blob/master/rofi.png)
## How to use
If necessary add `-font "yourfont size"` to the rofi command if the icons are not displaying properly  

### Print icon to terminal
```
curl -s https://raw.githubusercontent.com/groovykiwi/rofi-nerdfont/master/nerd-font-cheatsheet.txt | rofi -dmenu -p "NF Cheatsheet" -columns 2 -width 40 | cut -d" " -f1 | cat
```

### Copy icon to clipboard
```
curl -s https://raw.githubusercontent.com/groovykiwi/rofi-nerdfont/master/nerd-font-cheatsheet.txt | rofi -dmenu -p "NF Cheatsheet" -columns 2 -width 40 | cut -d" " -f1 | tr '\n' ' ' | xclip -selection clipboard
```

### Bash Script
It would be easier to use if you made a custom bash script and added it to your $PATH  
Additionally download the cheatsheet to prevent the delay caused by curl downloading it everytime. 
