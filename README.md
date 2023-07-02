# Install last versions of Nvim for ubuntu
I try install nvim in ubuntu but is old 6.X or thing and nvim-AppImage don't work with me

## Install nvim
firs you need to download nvim-linux64.tar.gz from 
https://github.com/neovim/neovim/releases

after download the file you need to extract the file
use this command `tar xzvf nvim-linux64.tar.gz`
don't forgot delet the `nvim-linux64.tar.gz` afte the extract

now you need to use this command `ln -s nvim-linux64/lib/nvim/ nvim`

now open nvim `./nvim`

if nvim open you do it now you need some simle things

## setup the the path for nvim 
you can use any path you want I chose `.local/bin` in home
after you chose the path you need to tell the linux you will use it
use any text editer you want and open this path `.bashrc` like this `my-text-editer ~/.bashrc`
and add this line 
```
# Add bin to PATH for my nvim 
PATH=$PATH:/home/$user/.local/bin
```
after that move the files to the path like this `mv nvim-linux64.tar.gz nvim ~/.local/bin`

and close the terminal and open it agan and open nvim like this `nvim`
