# Vim with Golang
Go언어와 Vim을 함께 쉽게 쓸 수 있도록 제가 세팅했던 내용들을 기록합니다.

##  Installation vim-go
### Install pathogen
```shell
$ cd ~/.vim
$ mkdir autoload && mkdir bundle
$ cd auotoload && curl -LSso pathogen.vim https://tpo.pe/pathogen.vim
```
```
# ~/.vimrc

set nu
syn on
set backspace=indent,eol,start
set encoding=utf-8


execute pathogen#infect()
filetype plugin indent on
```

### Install vim-go
```shell
$ cd ~/.vim/bundle && git clone https://github.com/fatih/vim-go.git
$ brew install mercurial
```
Vim으로 진입하여 `:GoInstallBinaries` 입력하여서 필요한 패키지들을 설치해 주세요.

## 참고한 문서
- [Terminal에서의 golang 개발을 위한 vim-go 세팅하기](https://www.hahwul.com/2019/12/24/terminal-golang-vim-go/)
