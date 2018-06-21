---
layout: default
title: The Elephant Collective Checkout
---

<script src="https://js.chargebee.com/v2/chargebee.js"
        data-cb-site="elephantcollective"> </script>



<div class="valign-wrapper full-vh">
  <div class="full-width center-align">
    <div>
      <img class="logo" src="/assets/images/logo.png"/>
    </div>
    <div>
      <div class="full-width center-align">
        <div class="input-field col s12">
          <select>
            <option value="" disabled selected>Choose your billing period</option>
            <option value="the-herd">Monthly  $25</option>
            <option value="the-herd-monthly">6 Months $125</option>
            <option value="the-herd">Yearly   $200</option>
          </select>
          <label>Period</label>
        </div>
        <div class="input-field col s12">
          <select>
            <option value="" disabled selected>Would you like to make an additional donation?</option>
            <option value="5">5</option>
            <option value="10">6 Months $125</option>
            <option value="15">Yearly   $200</option>
          </select>
          <label>Donation</label>
        </div>
      </div>

      <div>
        <a class="btn waves-effect waves-light pink"
           href="javascript:void(0)"
           data-cb-type="checkout"
           data-cb-plan-id="the-herd">
          Subscribe
        </a>
      </div>
      <div>
        <a href="javascript:void(0)"
           data-cb-type="portal">
          Manage Account
        </a>
      </div>
    </div>
  </div>
</div>

<script>
  $(document).ready(function(){
    $('select').formSelect();
    $('.dropdown-trigger').dropdown();
  });
</script>
