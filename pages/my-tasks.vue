<template>
    <section class="my-tasks page-tasks">
      <div class="custom-container">
        <myTaksWelcome />
        <accordion />
      </div>
    </section>
</template>

<script>
import myTaksWelcome from "../components/my-tasks/welcome";
import accordion from "../components/my-tasks/accordion";
export default {
   components:{myTaksWelcome,accordion},
  data() {
    return {};
  }
};
</script>

<style lang="scss">
.header {
  position: relative;
  background: #282929;
  background-image: url("https://epics.ieee.org/wp-content/uploads/2016/08/bigstock-Diverse-Architect-People-Group-98046365.jpg");
  background-size: cover;
  background-position-x: right;
  background-position-y: 460px;
  &:after {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, #292928e3, #000c40f0);
    left: 0;
    top: 0;
    z-index: -1;
  }
}
.my-tasks{
       background-color: #f1f1f1;
}
</style>
