+++
author = "Wamo"
date = 2020-01-04T15:00:00Z
description = "Donations from individuals / organizations, etc."
image = "/images/backgrounds/bg-2.jpg"
title = "Request for donation"

+++
<script src="https://js.stripe.com/v3"></script>

We are soliciting donations for future production activities and system operations.

Donations are made through Stripe.The amount that can be donated is 500¥/1000¥/5000¥.

No special benefits are planned for those who donate.
<!--more-->
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