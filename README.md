# Pix payment processing with Checkout API
[Português](README.pt.md) / [Español](README.es.md)

**:warning: Attention: Pix is a payment method only available in Brazil**

## :computer: Technologies
- PHP 7.3.29
- Slim Framework v4
- [Composer](https://getcomposer.org/download) (dependency manager)

## 💡 Requirements
- PHP 7.2.5 or higher (you can download PHP [here](https://www.php.net/downloads)).
- [Composer](https://getcomposer.org/download) (dependency manager).
- [Read our instructions](https://www.mercadopago.com.br/developers/en/guides/overview#bookmark_el_desarrollo_con_c%C3%B3digo) on how to create an application at the Mercado Pago Developer Panel in order to acquire your access token. It will grant you access to Mercado Pago's public APIs.
- For detailed information about receiving payments with Pix, [please read our guide](https://www.mercadopago.com.br/developers/en/guides/online-payments/checkout-api/other-payment-ways#bookmark_receive_payments_with_pix) at Mercado Pago Developers.

## :gear: Installation
1. Clone the project.
```bash
git clone https://github.com/mercadopago/pix-payment-sample-php.git
```

2. Go to the `server` folder.
```bash
cd pix-payment-sample-php/server
```

3. Install the required dependencies using Composer.
```bash
composer install
```

## 🌟 How to run it
1. Go to the `server` folder.
```bash
cd pix-payment-sample-php/server
```

2. Run the following command to start the application:
```bash
MERCADO_PAGO_SAMPLE_ACCESS_TOKEN=YOUR_ACCESS_TOKEN php -S localhost:8080 server.php
```

3. Remember to replace the value of `YOUR_ACCESS_TOKEN` with the corresponding [credential](https://www.mercadopago.com.br/developers/panel) from your account.

4. Navigate to http://localhost:8080 in your browser.

### :test_tube: Testing
- On our [testing instructions](https://www.mercadopago.com.br/developers/en/guides/online-payments/checkout-api/testing) you'll find a guide on how to create **[test users](https://www.mercadopago.com.br/developers/en/guides/online-payments/checkout-api/testing#bookmark_how_to_create_users)**.
- You have to [create a Pix key](https://www.mercadopago.com.br/stop/pix) in the seller's account in Mercado Pago (remember you can create and use a test user as a seller).
- **IMPORTANT:** there are some limitations when testing this payment method with test users. When creating a payment, it will be pending and the corresponding Pix code and QR code will be returned, but it will not be possible to use these codes to end the flow and approve the test payment.

## :handshake: Contributing
You can contribute to this project by reporting problems and bugs. Before opening an issue, make sure to read our [code of conduct](CODE_OF_CONDUCT.md).

## :bookmark: License
MIT License. Copyright (c) 2021 - Mercado Pago <br/>
For more information, see the [LICENSE](LICENSE) file.
