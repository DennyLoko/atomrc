# dotatom

This project contains the configuration and packages I use on my [Atom](https://atom.io/)

## Install packages
To install the packages on the `packages.list` file run:

```
apm install --packages-file packages.list
```

## Update packages list
To update the `packages.list` with the new version of the updated packages, simply run:

```
apm list --installed --bare > packages.list
```

## PANIC suggestion on atocomplete-go
Sometimes when you update to a new version of Go, [`gocode`](https://github.com/nsf/gocode) is not able to give appropriate suggestions, so it throws a panic. Thankfully the maintainers of `gocode` are very responsive, so when you do encounter this error, run the following command:

```
gocode close && go get -u github.com/nsf/gocode
```
