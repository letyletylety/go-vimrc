#VIMRC for Go

당연히 .vimrc로 바꿔서 사용해야 합니다.

```
git clone https://github.com/letyletylety/go-vimrc.git
mv vimrc ~/.vimrc
```

---

**키맵에서 au 로 시작하는 주석 2줄은 linux 기반 환경에서 캡스락과 esc를 바꾸는 방법입니다.**

```vimscript
au VimEnter * !xmodmap -e 'clear Lock' -e 'keycode 0x42 = Escape'
au VimLeave * !xmodmap -e 'clear Lock' -e 'keycode 0x42 = Caps_Lock'
```
