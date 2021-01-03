    <template>
  <b-navbar class="section">
    <template slot="brand">
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
        <img src="../assets/logo.png" alt="icoffex logo" />
      </b-navbar-item>
      <b-navbar-item class="to-right" slot="end" tag="div">
        <div class="">
          <div class="block">
            <b-icon icon="account-multiple-plus" size="is-medium"> </b-icon>
            <b-icon icon="magnify" size="is-medium"> </b-icon>
            <b-icon icon="cart" size="is-medium"> </b-icon>
          </div>
        </div>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script>
</script>

<style scoped>
.section {
  padding:1.2rem !important;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #4293b9;
}
.p-1 {
  padding: 1em;
}
a {
  margin-right: 1rem;
}
.to-right {
  position: absolute;
  right: 40px;
}
span {
  margin-left: 1rem;
  cursor: pointer;
}
span:hover {
  color: #d43d0e;
}
</style>
