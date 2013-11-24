##  Upgrading from 1.1.x

*    `$http` promises are now fully exposed for `$resource`
    *    Can be accessed via `$promise` after call
*    `_` is reserved for private properties
    *    i.e.
        *    Not inherited via `$scope` inheritance
        *    Not recognized via `$parse`
    *    Reversed in `1.2.1`
