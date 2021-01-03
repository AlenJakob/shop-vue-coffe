<template>
  <div class="columns section my-4">
    <div class="column content shiping-info-cart">
      <div class="columns">
        <div class="column is-2">
          <b-icon class="scoped-ico" icon="truck" size="is-medium"> </b-icon>
        </div>
        <div class="column">
          <p class="is-uppercase info has-text-left">24/7 CUSTOMER SERVICE</p>
          <p class="article has-text-left">
            Lorem ipsum dolor sit amet consectetur.
          </p>
        </div>
      </div>
    </div>

    <div class="column content shiping-info-cart">
      <div class="columns">
        <div class="column is-2">
          <b-icon class="scoped-ico" icon="headset" size="is-medium"> </b-icon>
        </div>
        <div class="column">
          <p class="is-uppercase info has-text-left">24/7 CUSTOMER SERVICE</p>
          <p class="article has-text-left">
            Lorem ipsum dolor sit amet consectetur.
          </p>
        </div>
      </div>
    </div>

    <div class="column content shiping-info-cart">
      <div class="columns">
        <div class="column is-2">
          <b-icon class="scoped-ico" icon="autorenew" size="is-medium">
          </b-icon>
        </div>
        <div class="column">
          <p class="is-uppercase info has-text-left">24/7 CUSTOMER SERVICE</p>
          <p class="article has-text-left">
            Lorem ipsum dolor sit amet consectetur.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style >
.info {
  font-size: 14px !important;
  font-weight: 600;
  line-height: 14px;
  color: rgb(75, 27, 0);
}
.article {
  line-height: 18px;
  margin-top: 11px;
  color: #682f0f;
}
.scoped-ico {
  color: rgb(58, 23, 0);
}
.shiping-info-cart:hover .scoped-ico {
    color:#d43d0e;
    
}
.shiping-info-cart{
    cursor: pointer;
}
</style>