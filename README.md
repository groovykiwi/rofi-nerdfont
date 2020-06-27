# Rofi Nerd Font Cheatsheet
## How to use

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
