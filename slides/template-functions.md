##  Template functions

*    Easier mechanism for applying conditional templates
*    When defining a directive, `template` key can take a function or a string
*    ex.
            return {
              template: function (element, attrs) {
                var html;
                if (attrs.trigger) {
                  html = '<div>Foo</div>';
                }
                else {
                  html = '<div>Bar</div>';
                }

                return html;
              }
            };
*    `templateUrl` also takes a similar function or string
