<template>
    <div class="content">
        <div class="account-ds">
            <div class="bar bar-nav account-top-m">
                <router-link to="/customer/account/index"  class="button button-link button-nav pull-left">
                    <span class="icon icon-left"></span>
                </router-link>
                <h1 class='title'>{{ $t("message.reset_password_success") }}</h1>
            </div>
        </div>
        <div class="fecshop_message" v-if="errormsg">
            <div class="error-msg">
                <div>
                    {{errormsg}}
                </div>
            </div>
		</div>
        <div class="fecshop_message" v-if="correctmsg">
            <div class="correct-msg">
                <div>
                    {{correctmsg}}
                </div>
            </div>
		</div>	
        
        <div class="customer-forgot-success">
            {{ $t("message.reset_accout_success") }} 
            <router-link to="/customer/account/login" >
                {{ $t("message.click_here") }}
            </router-link>
            {{ $t("message.to_login") }} .
        </div>
    </div>
</template>
<script>
export default {
    data () {
        return {
    
        }
    }
}
</script>