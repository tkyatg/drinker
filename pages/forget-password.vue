<template>
  <div class="auth">
    <div class="container pt-1">
      <el-row type="flex" class="row-bg" justify="center">
        <el-col :xs="24" :sm="16" :md="9">
          <el-card class="my-2 p-3" :body-style="{ padding: '0px' }">
            <el-row type="flex" class="row-bg" justify="center">
              <el-col :xs="24" :sm="24" :md="24">
                <div class="title">Password Reset!</div>
              </el-col>
            </el-row>
            <el-row type="flex" class="row-bg" justify="center">
              <el-col :xs="24" :sm="24" :md="24">
                <el-form class="login-form">
                  <el-form-item class="my-1">
                    <el-input placeholder="メールアドレス" v-model="email"></el-input>
                  </el-form-item>
                  <el-form-item class="text-center mt-2">
                    <el-button type="primary" >メール送信</el-button>
                  </el-form-item>
                </el-form>
                <hr>
                <div class="auth-link">
                  <NuxtLink to="/login">ログイン画面に戻る</NuxtLink>
                </div>
              </el-col>
            </el-row>
          </el-card>
        </el-col>
      </el-row>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      tableData: [{
        id:'1',
        detail: 'クレジットの購入',
        date:'2020-10-24',
        credit: '+300',
      },
      {
        id:`2`,
        detail: 'A子さんとの飲み',
        date:'2020-10-24',
        credit: '-400',
      }]
    }
  }
}
</script>
