<template>
  <div class="container">
    <div class="row">
      <div class="col-md-12 col-lg-12 col-xs-12 col-sm-12">
        <div class="row">
          <div class="col-md-6 col-xs-6 col-sm-6 col-lg-6 mt-4">
            <div class="row">
              <div class="col-md-10">
                <div class="progress progress-line">
                  <div
                    class="progress-bar progress-bar-line"
                    role="progressbar"
                    style="width: 90%"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
              <div class="col-md-2 text-left">
                <p class="progress_title">90%</p>
              </div>
            </div>
            <div class="row">
              <div class="col-md-10">
                <div class="progress progress-line">
                  <div
                    class="progress-bar green"
                    role="progressbar"
                    style="width: 90%"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
              <div class="col-md-2 text-left">
                <p class="progress_title"><i class="fa fa-check chk"></i></p>
              </div>
            </div>
            <div class="row">
              <div class="col-md-10">
                <div class="progress progress-line">
                  <div
                    class="progress-bar danger"
                    role="progressbar"
                    style="width: 90%"
                    aria-valuenow="90"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
              <div class="col-md-2 text-left">
                <p class="progress_title"><i class="fa fa-times cut"></i></p>
              </div>
            </div>
          </div>
          <div class="col-md-6 col-xs-6 col-sm-6 col-lg-6">
            <div class="row">
              <div class="col-md-4 col-lg-4">
                <div class="circle-wrap">
                  <div class="circle">
                    <div class="mask full">
                      <div class="fill"></div>
                    </div>

                    <div class="mask half">
                      <div class="fill"></div>
                    </div>

                    <div class="inside-circle">70%</div>
                  </div>
                </div>
              </div>
              <div class="col-md-4 col-lg-4">
                <div class="circle-wrap-g">
                  <div class="circle">
                    <div class="mask full">
                      <div class="fill"></div>
                    </div>

                    <div class="mask half">
                      <div class="fill"></div>
                    </div>

                    <div class="inside-circle"><i class="fa fa-check"></i></div>
                  </div>
                </div>
              </div>
              <div class="col-md-4 col-lg-4">
                <div class="circle-wrap-d">
                  <div class="circle">
                    <div class="mask full">
                      <div class="fill"></div>
                    </div>

                    <div class="mask half">
                      <div class="fill"></div>
                    </div>

                    <div class="inside-circle">!</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p.progress_title {
  font-size: 12px;
}
.progress-bar-line {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-direction: column;
  flex-direction: column;
  -ms-flex-pack: center;
  justify-content: center;
  overflow: hidden;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  background-color: #007bff;
  transition: width 0.6s ease;
  border-radius: 10px;
}
.progress-line {
  display: -ms-flexbox;
  display: flex;
  height: 1rem;
  overflow: hidden;
  line-height: 0;
  font-size: 0.75rem;
  background-color: #e9ecef;
  border-radius: 10px;
}
.green {
  background-color: #61c628 !important;
  border-radius: 10px;
}
.danger {
  background-color: #f2494d !important;
  border-radius: 10px;
}
.chk::before {
  background-color: #61c628;
  padding: 2px;
  border-radius: 10px;
  color: white;
}
.cut::before {
  background-color: #f2494d;
  padding: 2px 4px 3px 4px;
  border-radius: 10px;
  color: white;
  font-size: 10px;
}

/* circular bar */

.circle-wrap {
  margin: 0px auto;
  width: 150px;
  height: 150px;
  background: #e6e2e7;
  border-radius: 50%;
}

.circle-wrap .circle .mask,
.circle-wrap .circle .fill {
  width: 150px;
  height: 150px;
  position: absolute;
  border-radius: 50%;
}
.circle-wrap .circle .mask {
  clip: rect(0px, 150px, 150px, 75px);
}
.circle-wrap .circle .mask .fill {
  clip: rect(0px, 75px, 150px, 0px);
  background-color: #3daaaa;
}
.circle-wrap .circle .mask.full,
.circle-wrap .circle .fill {
  animation: fill ease-in-out 3s;
  transform: rotate(126deg);
}
.circle-wrap .inside-circle {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  background: #fff;
  line-height: 130px;
  text-align: center;
  margin-top: 10px;
  margin-left: 10px;
  position: absolute;
  z-index: 100;
  font-weight: 100;
  font-size: 12px;
}

.circle-wrap {
  margin: 0px auto;
  width: 150px;
  height: 150px;
  background: #e6e2e7;
  border-radius: 50%;
}

.circle-wrap .circle .mask,
.circle-wrap .circle .fill {
  width: 150px;
  height: 150px;
  position: absolute;
  border-radius: 50%;
}
.circle-wrap .circle .mask {
  clip: rect(0px, 150px, 150px, 75px);
}
.circle-wrap .circle .mask .fill {
  clip: rect(0px, 75px, 150px, 0px);
  background-color: #3daaaa;
}
.circle-wrap .circle .mask.full,
.circle-wrap .circle .fill {
  animation: fill ease-in-out 3s;
  transform: rotate(126deg);
}
.circle-wrap .inside-circle {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  background: #fff;
  line-height: 130px;
  text-align: center;
  margin-top: 10px;
  margin-left: 10px;
  position: absolute;
  z-index: 100;
  font-weight: 100;
  font-size: 12px;
}

.circle-wrap-g {
  margin: 0px auto;
  width: 150px;
  height: 150px;
  background: #e6e2e7;
  border-radius: 50%;
}

.circle-wrap-g .circle .mask,
.circle-wrap-g .circle .fill {
  width: 150px;
  height: 150px;
  position: absolute;
  border-radius: 50%;
}
.circle-wrap-g .circle .mask {
  clip: rect(0px, 150px, 150px, 75px);
}
.circle-wrap-g .circle .mask .fill {
  clip: rect(0px, 75px, 150px, 0px);
  background-color: #f2494d;
}
.circle-wrap-g .circle .mask.full,
.circle-wrap-g .circle .fill {
  animation: fill ease-in-out 3s;
  transform: rotate(126deg);
}
.circle-wrap-g .inside-circle {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  background: #fff;
  line-height: 130px;
  text-align: center;
  margin-top: 10px;
  margin-left: 10px;
  position: absolute;
  z-index: 100;
  font-weight: 100;
  font-size: 12px;
}

.circle-wrap-d {
  margin: 0px auto;
  width: 150px;
  height: 150px;
  background: #e6e2e7;
  border-radius: 50%;
}

.circle-wrap-d .circle .mask,
.circle-wrap-d .circle .fill {
  width: 150px;
  height: 150px;
  position: absolute;
  border-radius: 50%;
}
.circle-wrap-d .circle .mask {
  clip: rect(0px, 150px, 150px, 75px);
}
.circle-wrap-d .circle .mask .fill {
  clip: rect(0px, 75px, 150px, 0px);
  background-color: #61c628;
}
.circle-wrap-d .circle .mask.full,
.circle-wrap-d .circle .fill {
  animation: fill ease-in-out 3s;
  transform: rotate(126deg);
}
.circle-wrap-d .inside-circle {
  width: 130px;
  height: 130px;
  border-radius: 50%;
  background: #fff;
  line-height: 130px;
  text-align: center;
  margin-top: 10px;
  margin-left: 10px;
  position: absolute;
  z-index: 100;
  font-weight: 100;
  font-size: 12px;
}
</style>
