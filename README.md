# 🍔 Lazyswy

It uses fzf under the hood. You can use it for

- Switch between tmux sessions
- Create tmux sessions with preconfigured tmux windows

## 🍁 Installation

Install my-project with git

```bash
git clone https://github.com/alicemarple/lazyswy.git
cd lazyswy
cp ./lz ~/.local/bin/
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc
mkdir -p ~/.config/tmux/plugins/lazyswy/
cp ./lazyswy_dir ./lazyswy_flags.toml ~/.config/tmux/plugins/lazyswy/
```

Give permissions if needed

```bash
sudo chmod +x ~/.config/tmux/plugins/lazyswy/lazyswy_dir
sudo chmod +x ~/.local/bin/lz
```

### 🪴 How to use

Create tmux session in your project directory with fzf

```
lz
```

list running tmux sessions and switch to it. It also works in tmux session

```
lz -l
```

Create tmux session with preconfigured windows for developement

```
lz -d
```

Create tmux session with preconfigured windows for cybersecurity

```
lz -c
```

To flags like -d, -c use lazyswy_flags.toml file

### 🌸 Related

Here are related tools
[fzf](https://github.com/junegunn/fzf),
[tmux](https://github.com/tmux/tmux).
