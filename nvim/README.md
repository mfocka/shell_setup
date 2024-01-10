Starting out with nvchad.

first, backup existing nvim config:

```bash
mv ~/.config/nvim ~/.config/nvim.backup
rm -rf ~/.local/share/nvim
```

then install nvchad:
```bash
git clone https://github.com/NvChad/NvChad ~/.config/nvim --depth 1

nvim
```

You will now be prompted with "Do you want to install example custom config?", make sure to type in "N". Now, the lazy vim installer should start.

Once done, we will install a better theme. Do this by pressing `space t h` to open the **theme switcher"**. Choose the theme you like. I picked "catpuccin" and hit `enter`.

now we will start to make the nvim environment perfect for c++.
We will start with autosuggestions and code completion. This can be done by adding an lsp server. The preference is clangd.

We will install the plugins using neovim itself by using a plugin called mason. This is a package manager.

To do this, open `nvim`, then do `ctrl n` to open the file explorer. Go to "lua/custom/chadrc.lua" and add the following line:
```lua
M.plugins = "custom.plugins"
```
then, create a new file (`ctrl h` then `a`) named "plugins.lua" and add the plugins you want.
This looks something like:
```nvim
ensure_installed = {
    "clangd",
    "gopls",
    "rust-analyzer",
}
```
