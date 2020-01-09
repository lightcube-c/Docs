+++
author = "Wamo"
date = 2020-01-04T15:00:00Z
description = "個人/団体からの寄付など"
image = "/images/backgrounds/bg-2.jpg"
title = "寄付のお願い"

+++
<script src="https://js.stripe.com/v3"></script>
私たちは、今後の制作活動やシステム面での運用で、寄付を募っております。

寄付は、Stripeを通じて行われます。寄付できる金額は、500¥/1000¥/5000¥となっております。

寄付をしてくださった方に対する特典などは2020年1月現在予定しておりません。
<!--more-->
なお、お支払方法は、クレジットカード（Visa・Mastercard・AmericanExpress）のみです。

<br>
<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_GUtBGGKzxtNvRZ"
  role="link"
>
  Bronze - 500&yen;
</button>

<div id="error-message"></div>

<script>
(function() {
  var stripe = Stripe('pk_live_pr925QBVIDmhyp46e2xgaX5a00zG0BtTNS');

  var checkoutButton = document.getElementById('checkout-button-sku_GUtBGGKzxtNvRZ');
  checkoutButton.addEventListener('click', function () {
    stripe.redirectToCheckout({
      items: [{sku: 'sku_GUtBGGKzxtNvRZ', quantity: 1}],
      successUrl: 'https://lightcube.netlify.com/',
      cancelUrl: 'https://lightcube.netlify.com/',
    })
    .then(function (result) {
      if (result.error) {
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
})();
</script>
<br>
<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_GUtBA1AlxpXxDG"
  role="link"
>
  Silver - 1000&yen;
</button>

<div id="error-message"></div>

<script>
(function() {
  var stripe = Stripe('pk_live_pr925QBVIDmhyp46e2xgaX5a00zG0BtTNS');

  var checkoutButton = document.getElementById('checkout-button-sku_GUtBA1AlxpXxDG');
  checkoutButton.addEventListener('click', function () {
    stripe.redirectToCheckout({
      items: [{sku: 'sku_GUtBA1AlxpXxDG', quantity: 1}],
      successUrl: 'https://lightcube.netlify.com/',
      cancelUrl: 'https://lightcube.netlify.com/',
    })
    .then(function (result) {
      if (result.error) {
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
})();
</script>
<br>
<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-sku_GUtBln7RveVpx6"
  role="link"
>
  Gold - 5000&yen;
</button>

<div id="error-message"></div>

<script>
(function() {
  var stripe = Stripe('pk_live_pr925QBVIDmhyp46e2xgaX5a00zG0BtTNS');

  var checkoutButton = document.getElementById('checkout-button-sku_GUtBln7RveVpx6');
  checkoutButton.addEventListener('click', function () {
    stripe.redirectToCheckout({
      items: [{sku: 'sku_GUtBln7RveVpx6', quantity: 1}],
      successUrl: 'https://lightcube.netlify.com/',
      cancelUrl: 'https://lightcube.netlify.com/',
    })
    .then(function (result) {
      if (result.error) {
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
})();
</script>
