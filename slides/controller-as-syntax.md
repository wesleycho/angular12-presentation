##  `Controller as` Syntax

*    Can namespace methods as part of a controller
    *    ex.
                <div ng-controller="DemoCtrl as Demo"></div>
*    Used essentially as an isolated scope
    *    ex.
                <div ng-class="{active: Demo.hasClass(item)}"></div>
*    Methods attached to the controller do not get inherited by child scopes
    *    ex.
                function DemoCtrl ($scope) {
                    this.hasClass = function (item) {
                        item.id === 1 ? return true : return false;
                    };
                }

