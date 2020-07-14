# Rofi Nerd Font Cheatsheet
![Picture](https://github.com/groovykiwi/rofi-nerdfont/blob/master/rofi.png)
## How to use
If necessary add `-font "yourfont size"` to the rofi command if the icons are not displaying properly   
  
~~Some icons cause rofi to mess up the alignment and put them all the way to the left, shouldn't affect the script but still to be noted~~  
Issue was resolved by adding a blank braille character at the beginning of each new line and deleting it after selection.


### Print icon to terminal
```
curl -s https://raw.githubusercontent.com/groovykiwi/rofi-nerdfont/master/nerd-font-cheatsheet.txt | rofi -dmenu -p "NF Cheatsheet" -columns 2 -width 40 | cut -d" " -f1 | sed 's/⠀//g; s/\s//g' | cat
```

### Copy icon to clipboard
```
curl -s https://raw.githubusercontent.com/groovykiwi/rofi-nerdfont/master/nerd-font-cheatsheet.txt | rofi -dmenu -p "NF Cheatsheet" -columns 2 -width 40 | cut -d" " -f1 | tr '\n' ' ' | sed 's/⠀//g; s/\s//g' | xclip -selection clipboard
```

### Bash Script
It would be easier to use if you made a custom bash script and added it to your $PATH  
Additionally download the cheatsheet to prevent the delay caused by curl downloading it everytime. 
