## Perl-TestMore-Selenium

This code is provided on an "AS-IS” basis without warranty of any kind, either express or implied, including without limitation any implied warranties of condition, uninterrupted use, merchantability, fitness for a particular purpose, or non-infringement. Your tests and testing environments may require you to modify this framework. Issues regarding this framework should be submitted through GitHub. For questions regarding Sauce Labs integration, please see the Sauce Labs documentation at https://wiki.saucelabs.com/. This framework is not maintained by Sauce Labs Support.

### Environment Setup

1. Global Dependencies
    * Install [PHP](https://www.perl.org/get.html)

2. Sauce Credentials
    * In the terminal export your Sauce Labs Credentials as environmental variables:
    ```
    $ export SAUCE_USERNAME=<your Sauce Labs username>
	$ export SAUCE_ACCESS_KEY=<your Sauce Labs access key>
    ```
3. Project Dependencies
	* Install packages (sudo may be necessary)
	```
	$ cpan -i Test::More
    $ cpan -i JSON
    $ cpan -i Env
    $ cpan -i Selenium::Remote::Driver
    $ cpan -i LWP::UserAgent
    $ cpan -i HTTP::Request
	```

### Running Tests

* Tests in Parallel:
	```
	$ make run_all_in_parallel
	```
[Sauce Labs Dashboard](https://saucelabs.com/beta/dashboard/)

### Advice/Troubleshooting

1. There may be additional latency when using a remote webdriver to run tests on Sauce Labs. Timeouts or Waits may need to be increased.
    * [Selenium tips regarding explicit waits](https://wiki.saucelabs.com/display/DOCS/Best+Practice%3A+Use+Explicit+Waits)

### Resources
##### [Sauce Labs Documentation](https://wiki.saucelabs.com/)

##### [SeleniumHQ Documentation](http://www.seleniumhq.org/docs/)

##### [TestMore Documentation](http://perldoc.perl.org/Test/More.html)

##### [CPAN Documentation](http://search.cpan.org/~andk/CPAN-2.10/lib/CPAN.pm)

##### [Stack Overflow](http://stackoverflow.com/)
* A great resource to search for issues not explicitly covered by documentation
