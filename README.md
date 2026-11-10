> [!WARNING]
> **This repository is archived and no longer maintained by BitPay.**
>
> It is read-only and will not receive updates, bug fixes, or security fixes. Please do not start new integrations from this code.
>
> For currently supported integrations, see [eCommerce Plugins](https://developer.bitpay.com/docs/plugins) and [Libraries](https://developer.bitpay.com/docs/libraries). If you already use this code, we recommend moving to a supported integration.

# Description

Bitcoin payment plugin for Ecwid using the bitpay.com service.


## Quick Start Guide

* Last Version Tested: 13.0.1629

To get up and running with our plugin quickly, see the GUIDE here: https://github.com/bitpay/ecwid-plugin/blob/master/GUIDE.md


## Troubleshooting

The official BitPay API documentation should always be your first reference for development: https://bitpay.com/downloads/bitpayApi.pdf

- Verify that your "notificationURL" for the invoice is "https://" (not "http://")
- Ensure a valid SSL certificate is installed on your server. Also ensure your root CA cert is updated. If your CA cert is not current, you will see curl SSL verification errors.
- Verify that your callback handler at the "notificationURL" is properly receiving POSTs. You can verify this by POSTing your own messages to the server from a tool like Chrome Postman.
- Verify that the POST data received is properly parsed and that the logic that updates the order status on the merchants web server is correct.
- Verify that the merchants web server is not blocking POSTs from servers it may not recognize. Double check this on the firewall as well, if one is being used.
- Use the logging functionality to log errors during development. If you contact BitPay support, they will ask to see the log file to help diagnose any problems.
- Check the version of this plugin against the official repository to ensure you are using the latest version. Your issue might have been addressed in a newer version of the library.

## Support
 
**BitPay Support:**

* [GitHub Issues](https://github.com/bitpay/ecwid-plugin/issues)
  * Open an issue if you are having issues with this plugin.
* [Support](https://help.bitpay.com/)
  * BitPay merchant support documentation

**Ecwid Support**

* [Homepage](https://www.ecwid.com/)
* [Documentation](https://help.ecwid.com/)
* [Support](https://help.ecwid.com/customer/portal/emails/new)

## Version History

- Bitpay plugin version 1.0
- Tested against Ecwid version 13.0.1629
- Added new HTTP header for version tracking

## License

©2011-2015 BITPAY, INC.

The MIT License (MIT)

Permission is hereby granted to any person obtaining a copy of this software and associated documentation for use and/or modification in association with the bitpay.com service.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

