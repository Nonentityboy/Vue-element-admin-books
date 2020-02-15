<template>
  <div class="detail">
    <el-form ref="postForm" :model="postForm" :rules="rules" class="form-container">
      <sticky :z-index="10" :class-name="'sub-navbar ' + postForm.status">
        <el-button v-if="!isEdit" @click.prevent.stop="showGuide">显示帮助</el-button>
        <el-button v-loading="loading" style="margin-left: 10px;" type="success" @click="submitForm">
          {{ isEdit ? '编辑电子书' : '新增电子书' }}
        </el-button>
      </sticky>
      <div class="detail-container">
        <el-row>
          <Warning />
          <el-col :span="24" />
          <el-col :span="24" />
        </el-row>
      </div>
    </el-form>
  </div>
</template>

<script>
export default {
  props: {
    isEdit: Boolean
  }
}
</script>

<style lang="scss" scoped>
  @import "~@/styles/mixin.scss";

  .detail {
    position: relative;
    .detail-container {
      padding: 40px 45px 20px 50px;
      .preview-img {
        width: 200px;
        height: 270px;
      }
      .contents-wrapper {
        padding: 5px 0;
      }
    }
  }
</style>
