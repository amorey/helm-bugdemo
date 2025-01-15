# helm-bugdemo

Example to show that importing `helm.sh/helm/v3/pkg/action` results in a warning when `go test -race` is run:

```
$ go test -race ./...
# helm-bugdemo.test
ld: warning: '/private/var/folders/x2/mygv_s3s0fj72cqn6tn8sphr0000gn/T/go-link-2763748380/000012.o' has malformed LC_DYSYMTAB, expected 98 undefined symbols to start at index 884, found 95 undefined symbols starting at index 884
ok  	helm-bugdemo	1.166s
```
