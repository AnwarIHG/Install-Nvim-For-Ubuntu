# Install latest version of Neovim for Ubuntu

If you are trying to install Neovim on Ubuntu and find that the available version is outdated (e.g., 6.X), or the `nvim-AppImage` doesn't work for you, follow these steps to install the latest version.

## Install Neovim

1. Download the latest version of Neovim for Linux. Go to the Neovim GitHub releases page: [https://github.com/neovim/neovim/releases](https://github.com/neovim/neovim/releases)

2. Download the `nvim-linux64.tar.gz` file from the latest release.

3. After the download is complete, extract the contents of the `nvim-linux64.tar.gz` file using the following command:

   ```bash
   tar xzvf nvim-linux64.tar.gz
   ```
Once the extraction is done, you can delete the **nvim-linux64.tar.gz** file.

Next, create a symbolic link to the *nvim* binary inside the extracted directory.
This allows you to execute Neovim from any location in the terminal.

```bash
ln -s /path/to/extracted/nvim-linux64/bin/nvim ~/.local/bin/nvim
```
Replace `/path/to/extracted` with the actual path to the directory where you extracted *Neovim*.

Now, you need to set up the PATH environment variable to include Neovim's binary location.
This step allows you to run *Neovim* simply by typing nvim in the terminal.

Open your `~/.bashrc` file (or `~/.bash_profile` if you are using it) in a text editor:

```bash
my-text-editor ~/.bashrc
```
Add the following line at the end of the file:

```bash
export PATH=$PATH:$HOME/.local/bin
```
Save the file and close the text editor.

Move the nvim binary to the chosen PATH, in this case ~/.local/bin:

```bash
mv nvim ~/.local/bin/
```
Close the terminal and open it again to apply the changes to the PATH environment variable.

Now you can open *Neovim* by simply typing `nvim` in the terminal.

With these steps, you should have successfully installed and set up the latest version of ***Neovim*** on your Ubuntu system. Happy coding!
