# Git & Oh My Zsh Configuration

This repository contains my personal Git and Oh My Zsh configurations, making it easy to sync settings across multiple machines.

## Contents

- `.gitconfig`: Git user settings, aliases, and configurations
- `.zshrc`: Oh My Zsh settings, theme configuration, plugins, and custom functions
- `custom/`: Additional custom Oh My Zsh scripts and configurations (if any)

## Installation

### Prerequisites

Before installing these configurations, make sure you have:

1. [Git](https://git-scm.com/downloads) installed
2. [Oh My Zsh](https://ohmyz.sh/#install) installed
3. [fzf](https://github.com/junegunn/fzf#installation) (optional, but recommended for the custom Git functions)

### Setup Instructions

1. **Backup your existing configurations**

   ```bash
   mv ~/.gitconfig ~/.gitconfig.bak
   mv ~/.zshrc ~/.zshrc.bak
   ```

2. **Clone this repository**

   ```bash
   git clone git@github.com:oaoxd0314/git-config.git ~/git-config
   ```

3. **Create symbolic links**

   ```bash
   ln -s ~/git-config/.gitconfig ~/.gitconfig
   ln -s ~/git-config/.zshrc ~/.zshrc
   ```

4. **Apply the changes**

   ```bash
   source ~/.zshrc
   ```

### Additional Dependencies

Depending on your specific configuration, you may need to install:

- **PNPM**: Follow the [official installation guide](https://pnpm.io/installation)
- **Python**: Install via [official website](https://www.python.org/downloads/) or package manager
- **Deno**: Follow the [official installation instructions](https://deno.land/#installation)

## Customization

Feel free to modify the configuration files to suit your needs. After making changes:

1. Commit your changes to the repository
   ```bash
   cd ~/git-config
   git add .
   git commit -m "Update configurations"
   git push
   ```

2. If you've added new custom scripts for Oh My Zsh, place them in the `custom/` directory and ensure they're properly linked in your setup.

## Syncing with Other Machines

To sync your configurations to another machine:

1. Clone this repository on the new machine
   ```bash
   git clone git@github.com:oaoxd0314/git-config.git ~/git-config
   ```

2. Follow the installation steps above
3. For updates, simply pull the latest changes:
   ```bash
   cd ~/git-config
   git pull
   ```

## Troubleshooting

- If you encounter any issues with the custom functions, make sure fzf is properly installed
- For path or environment variable issues, ensure that your system's core paths are not being overwritten
- If certain aliases or functions aren't working, check that the necessary plugins and dependencies are installed

## Maintenance

To keep your configurations in sync across all your machines:

1. Always commit and push changes from any machine where you update configurations
2. Regularly pull changes when switching to another machine
3. Consider reviewing and cleaning up old or unused configurations periodically

## License

This configuration is shared for personal use - feel free to fork and modify for your own purposes.

