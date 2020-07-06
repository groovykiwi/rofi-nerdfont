# Rofi Nerd Font Cheatsheet
## How to use
![Picture](https://github.com/groovykiwi/rofi-nerdfont/blob/master/rofi.png)
### Print icon to terminal
```
curl -s https://raw.githubusercontent.com/groovykiwi/rofi-nerdfont/master/nerd-font-cheatsheet.txt | rofi -dmenu -p "NF Cheatsheet" -columns 2 -width 40 | cut -d" " -f1 | cat
```

### Copy icon to clipboard
```
curl -s https://raw.githubusercontent.com/groovykiwi/rofi-nerdfont/master/nerd-font-cheatsheet.txt | rofi -dmenu -p "NF Cheatsheet" -columns 2 -width 40 | cut -d" " -f1 | tr '\n' ' ' | xclip -selection clipboard
```

### Bash Script
It would be easier to use if you made a custom bash script and added it to your PATH  
Additionally download the cheatsheet to prevent the delay caused by curl downloading it everytime. 
