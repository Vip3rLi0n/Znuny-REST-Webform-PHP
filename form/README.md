### Using the created php script to create ticket through webpage form.

News:
- ✅ Compatible with Znuny 6
- ✅ Using latest library
- ✅ Works with PHP7, PHP-FPM and PHP8.

### Requirements
- [Znuny](https://github.com/znuny/Znuny) version 6+
- [PHP](https://github.com/php) version 7+ with Composer
- Specific Agent account for Webservice usage

## Prepare your ticket system
- First, download the web service configuration from [GitHub](https://github.com/Ni3zam/Znuny-REST-Webform-PHP/raw/main/GenericTicketConnectorREST.yaml).
- Navigate as an admin to `Admin` => `Web Service Management` => `Add Web Service` => `Import web service`. Enter a name for the web service.
- I suggest to use `GenericTicketConnectorREST` because this is used in the example.

## Install example client
- Clone this repository and run `composer update` to add the [Unirest](https://github.com/apimatic/unirest-php) library:

```bash
$ git clone https://github.com/Ni3zam/Znuny-REST-Webform-PHP webform
$ cd webform
$ composer update
```

## Prepare the client
**Edit client.php and complete the baseURL and configure those listed below.**
- [FQDN](https://github.com/Ni3zam/znuny-gi-rest-php/blob/main/client.php#L11).
- [WebServiceName](https://github.com/Ni3zam/znuny-gi-rest-php/blob/main/client.php#L12).
- [UserLogin](https://github.com/Ni3zam/znuny-gi-rest-php/blob/main/client.php#L17).
- [Password](https://github.com/Ni3zam/znuny-gi-rest-php/blob/main/client.php#L18).

## Run your client
Your client is ready to go and can be executed by going to `/test.html`

### Misc
An introduction for the Generic Interface for the latest ((OTRS)) Community Editon is available in the [Online Manual](https://doc.otrs.com/doc/manual/admin/6.0/en/html/genericinterface.html).

The default operations TicketCreate and TicketUpdate are not able to send a **new** article via e-mail. For this use case you could install the free add-on [Znuny4OTRS-GIArticleSend](https://github.com/znuny/Znuny4OTRS-GIArticleSend).


### Credit
rkaldung: [Click Here](https://github.com/rkaldung/otrs-gi-rest-php)
