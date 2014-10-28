Change from standard library is listed below
====

    > diff -u /usr/local/go/src/pkg/bufio/scan.go scan.go
    --- /usr/local/go/src/pkg/bufio/scan.go 2014-08-12 20:52:26.000000000 -0700
    +++ scan.go 2014-11-01 17:33:25.000000000 -0700
    @@ -66,7 +66,7 @@
     const (
        // Maximum size used to buffer a token. The actual maximum token size
        // may be smaller as the buffer may need to include, for instance, a newline.
    -   MaxScanTokenSize = 64 * 1024
    +   MaxScanTokenSize = 64 * 1024 * 2
     )

     // NewScanner returns a new Scanner to read from r.

