This is a shim pointing at the original hover repo commit.

This allows to use an untagged commit of `hover` with `go get`, which normally should be avoided unless there is a problem with the latest tagged release.

```
# set GO111MODULE=on unless it's already in env
go get -u -a github.com/worldr/hover

# the original would be:
# go get -u -a github.com/go-flutter-desktop/hover
```

Use `hover` as you normally would, the shim is nothing but a reference.