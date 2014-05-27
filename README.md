# Puppet module: typo3 

This is a puppet module that installs typo3

Made by Daniel Paschke 

Released under the terms of Apache 2 License.

This module requires functions provided by the Example42 Puppi module (you need it even if you don't use and install Puppi)

## USAGE - Basic management

* Install typo3 with default settings (installs sources in /opt, the page in /var/www/typo3.loc)

        class { 'typo3': }

* Install a specific version of typo3

        class { 'typo3':
          version => '6.1.7',
        }

* Install special version (< 6.2.0) 

        class { 'typo3':
          version => '6.1.7',
          site_type => 'introductionpackage'
        }

* Install in a custom directory

        class { 'typo3':
          site_name => 'mytyposite.com' 
        }


