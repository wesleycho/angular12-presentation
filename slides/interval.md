##  $interval

*    Companion service to `setInterval`
*    Notifies with the count of each iteration of callback
*    ex.
            // You shouldn't do this!
            var polling = $interval(pollServer, 1000);
            polling.then(func1, func2, function (count) {
                console.log('Number of iterations of polling: '
                    + count);
            });
*    Works similarly to `$timeout`
