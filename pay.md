---
layout: default
title: The Herd Checkout
---

<script src="https://js.chargebee.com/v2/chargebee.js" data-cb-site="elephantcollective" ></script>

<div class="black-bg">
  <div class="valign-wrapper full-vh">
    <div class="full-width center-align">
      <div>
        <Img class="logo" src="/assets/img/logo/logo.png"/>
      </div>
      <div>
        <a id="checkout" href="javascript:void(0)" data-cb-type="checkout" data-cb-plan-id="the-herd" class="btn waves-effect waves-light pink">
          Subscribe to the Herd!
        </a>
      </div>
    </div>
  </div>
</div>

<script type="text/javascript">
  $(document).ready(function(){
  var params = $.deparam(location.search.replace("\?", ""));
  $("#checkout").attr("data-cb-coupon-id", params.coupon);
  Chargebee.registerAgain();
  });
</script>
