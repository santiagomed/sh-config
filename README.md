# Shell/Editor Configuration Setup

Welcome to the shell/editor configuration setup guide! In this guide, we will go through the steps to set up `oh-my-zsh` and the `starship` theme to enhance your terminal experience.

## Prerequisites

- A Unix-like operating system (macOS, Linux, WSL)
- `zsh` shell installed (you can check with `zsh --version`)
- `curl` installed (you can check with `curl --version`)

## Step-by-Step Setup

### Step 1: Install `oh-my-zsh`

1. **Backup Existing Configuration:**
   Before making any changes, it's a good idea to backup your current shell configuration.
   ```bash
   cp ~/.zshrc ~/.zshrc.backup
   ```

2. **Install `oh-my-zsh` via Command Line:**
   Open your terminal and run the following command:
   ```bash
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

   Follow the on-screen prompts to complete the installation.

### Step 2: Install the `starship` Prompt

1. **Install `starship`:**
   Run the following command in your terminal:
   ```bash
   curl -sS https://starship.rs/install.sh | sh
   ```

2. **Add `starship` to `.zshrc`:**
   Append the following line to the end of your `.zshrc` file to initialize `starship` with `zsh`:
   ```bash
   echo 'eval "$(starship init zsh)"' >> ~/.zshrc
   ```

### Step 3: Apply Changes

1. **Reload Shell Configuration:**
   To apply the changes you've made to your `.zshrc`, either restart your terminal or run:
   ```bash
   source ~/.zshrc
   ```

## Verification

To verify that everything has been set up correctly:

- Open a new terminal window.
- You should see the `starship` prompt along with any `oh-my-zsh` features.

## Customization

Feel free to customize the `starship` prompt to meet your needs by editing the `~/.config/starship.toml` file. You can find detailed configuration options in the [starship documentation](https://starship.rs/config/).

## Conclusion

Congratulations! You have successfully set up `oh-my-zsh` and the `starship` theme. Enjoy your personalized and powerful terminal experience! If you encounter any issues or have any questions, consult the official documentation for [oh-my-zsh](https://ohmyz.sh/) and [starship](https://starship.rs/).

---

Happy hacking! 🚀

---

*This guide was generated with ❤️ for developers seeking an enhanced terminal experience.*
