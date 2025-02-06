# PHP Timezone Bug
This repository demonstrates a common error related to timezone handling in PHP's `date()` function.  The default behavior of `date()` is to use the server's configured timezone, which can lead to incorrect results if the application needs to work with dates and times from various timezones.

The `bug.php` file shows the problematic code, while `bugSolution.php` provides a corrected version that utilizes the DateTimeZone class for proper timezone management.

## How to Reproduce
1. Clone this repository.
2. Run `bug.php`. Observe the output; it will likely be different from the input date string due to the server's timezone setting.
3. Run `bugSolution.php`.  Note the correct output reflecting the specified timezone.