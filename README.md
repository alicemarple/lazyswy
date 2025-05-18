# 🍔 Lazyswy

It uses fzf under the hood. You can use it for

- Switch between tmux sessions
- Create tmux sessions with preconfigured tmux windows
- List the sessions stored by the tmux-resurrect

## 🍁 Installation

Install my-project with git

```bash
git clone https://github.com/alicemarple/lazyswy.git
cd lazyswy
cp ./lzy ~/.local/bin/
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc
mkdir -p ~/.config/tmux/plugins/lazyswy/
cp ./lazyswy_dir ./lazyswy_flags.toml ~/.config/tmux/plugins/lazyswy/
```

Give permissions if needed

```bash
sudo chmod +x ~/.config/tmux/plugins/lazyswy/lazyswy_dir
sudo chmod +x ~/.local/bin/lzy
```

If you want to use tmux-resurrect list feature then add below line in your tmux config

```
set -g @resurrect-dir '~/.config/tmux/plugins/resurrect'
```

### 🪴 How to use

Create tmux session in your project directory with fzf

```
lzy
```

list running tmux sessions and switch to it. It also works in tmux session

```
lzy -l
```

List all sessions saved using tmux-resurrect

```
lzy -r
```

Create tmux session with preconfigured windows for developement

```
lzy -d
```

Create tmux session with preconfigured windows for cybersecurity

```
lzy -c
```

To flags like -d, -c use lazyswy_flags.toml file

### 🌸 Related

Here are related tools
[fzf](https://github.com/junegunn/fzf),
[tmux](https://github.com/tmux/tmux).
