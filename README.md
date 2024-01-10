# Terminal Configuration Setup

This repository contains configurations for a customized terminal setup using Zsh, Oh My Zsh, and the Powerlevel10k theme. This documentation is only focused on the folder **"ubuntu"**.

## Getting Started

Follow these steps to set up your terminal with the provided configuration:

### 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/mfocka/shell_setup.git
```

### 2. Copy Configuration Files
Copy the .zshrc file and the .oh-my-zsh directory from the cloned repository to your home directory:

```bash
cp your-terminal-config/.zshrc ~/
cp -r your-terminal-config/.oh-my-zsh/ ~/
```

#### 3. Install Zsh and Oh My Zsh

- **Install Zsh:** Ensure Zsh is installed on your machine. On Ubuntu, you can use:

```bash
sudo apt-get install zsh
```

- **Install Oh My Zsh:**

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### 4. Install Powerlevel10k Theme
Follow the instructions on the Powerlevel10k GitHub repository to install the theme:

- [Powerlevel10k Installation](https://github.com/romkatv/powerlevel10k#oh-my-zsh)
- If you want to skip learning about this and download it instead:
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
Check if the following flag is set:
```bash
Set ZSH_THEME="powerlevel10k/powerlevel10k" in ~/.zshrc.
```

### 5. Install Additional Plugins (if any)

If your configuration references additional plugins, install them using the package manager or following the plugin's instructions.

### 6. Restart or Reload Zsh
Restart your terminal or run the following command to apply the new configurations:

```bash
source ~/.zshrc
```

## Additional Notes
- If you encounter any issues, make sure to check the documentation for Zsh, Oh My Zsh, and Powerlevel10k for troubleshooting.
- Customize the configurations further based on your preferences.
  
Happy coding!
