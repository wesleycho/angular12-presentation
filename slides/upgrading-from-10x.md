##  Upgrading from 1.0.x

*    `$route` is split off
  *    Now resides in `angular-route.js`
  *    Need to include `ngRoute` as module dependency
*    `ng-bind-html-unsafe` is no more!
  *    Need to use `$sce` service from `ngSanitize`
  *    `ngSanitize` is found in `angular-sanitize.js`
  *    Need to explicitly whitelist HTML via `$sce.trustAsHtml`
*    `ng-repeat` may need usage of `track by` syntax
  *  i.e.
            ng-repeat="item in items track by $index"
