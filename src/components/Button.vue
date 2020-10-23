<template>
  <div class="container">
    <div class="row">
      <div class="col-md-12 col-lg-12 col-xs-12 col-sm-12">
        <div class="row">
          <div class="col-md-6 col-xs-6 col-sm-6 col-lg-6 mt-5">
            <!-- <div class="text-center">
              <div class="main">
                <button type="button" class="btn btn-bg">Button</button>

                <div class="bg-shadow">
                  <div class="d-flex">
                    <div class=""><span class="icon-bg">!</span></div>
                    <div class="data-bg ml-2">Tooltip for guided Tour</div>
                  </div>
                  <div class="d-flex justify-content-end">
                    <div class="d-flex mt-2">
                      <button type="button" class="btn btn-bg-yes">yes</button>
                      <button type="button" class="btn btn-bg-no ml-1">
                        no
                      </button>
                    </div>
                  </div>
                </div>
              </div>
            </div> -->

            <a
              class="link"
              target="_blank"
              draggable="false"
              data-tooltip="Tooltip uses experimental 'width: max-content', look it up on caniuse.com"
              >hover 1.2 seconds</a
            >
            <a href="#" target="_blank" draggable="false"
              ><abbr data-title="Look, a tooltip!">Hover me, too!</abbr></a
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Button",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.btn-bg {
  background-color: #10454e;
  color: white;
}
.bg-shadow {
  -webkit-box-shadow: 1px 1px 5px 0px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 1px 1px 5px 0px rgba(0, 0, 0, 0.75);
  box-shadow: 1px 1px 5px 0px rgba(0, 0, 0, 0.75);
  max-width: 250px;
  border-radius: 10px;
  padding: 10px;
  margin-top: 10px;
}
button.btn.btn-bg-no {
  background-color: #10454e;
  color: white;
}

button.btn.btn-bg-yes {
  border: solid 1px #10454e;
}
</style>
