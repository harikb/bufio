Change from standard library is listed below
====

        diff --git a/scan.go b/scan.go
        index 364d159..8cb2b16 100644
        --- a/scan.go
        +++ b/scan.go
        @@ -68,7 +68,7 @@ const (
                // MaxScanTokenSize is the maximum size used to buffer a token.
                // The actual maximum token size may be smaller as the buffer
                // may need to include, for instance, a newline.
        -       MaxScanTokenSize = 64 * 1024
        +       MaxScanTokenSize = 64 * 1024 * 1024
         )
        
         // NewScanner returns a new Scanner to read from r.
