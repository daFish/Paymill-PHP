# Paymill-PHP

[![Build Status](https://secure.travis-ci.org/Paymill/Paymill-PHP.png)](http://travis-ci.org/Paymill/Paymill-PHP)

# Getting started with Paymill

1.  Include the required PHP file from the paymill PHP library. For example via: 

        require_once 'lib/Services/Paymill/Transactions.php';

2.  Instantiate the class, for example the Services_Paymill_Transactions class, with the following parameters:

    $apiKey: First parameter is always your private API (test) Key

    $apiEndpoint: Second parameter is to configure the API Endpoint (with ending /), e.g. "https://api.paymill.de/v1/"
	
        $transactionsObject = new Services_Paymill_Transactions($apiKey, $apiEndpoint);

3.  Make the appropriate call on the class instance. For additional parameters please refer to the API-Reference:

        $transactionsObject->create($params);
	
For further information, please refer to our official PHP library reference:
http://paymill.de/documentation/referenz/api-referenz/
