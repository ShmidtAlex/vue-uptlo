<template>
	<div class="app-header">
		<div class="header">
		<nav class="navbar navbar-default navbar-fixed-top">
		  <div class="navbar-brand">
		    <a href=""><img src="../assets/UPTLO.png" alt=""></a>
		  </div>
		  <div class="login_block">
		    <button @click="open_loginform" type='button' class="login" data-target1="#modal-sidebar-login" data-toggle1="modal">login</button>
		    <button  type='button' class="sign_up" data-toggle="modal" data-target="#modal-sidebar-signup">sign up</button>
		  </div>              
		  <div class="container">
		    <div class="navbar-header">
		      <!--кнопка-гамбургер-->
		      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar_collapse_1" aria-expanded='false'>  
		        <span class="sr-only">Toggle navigation</span>
		        <span class="icon-bar"></span>
		        <span class="icon-bar"></span>
		        <span class="icon-bar"></span>    
		      </button>
		    </div>
		    <!-- выпадающее меню на маленьких устройствах-->
		    <div class="collapse navbar-collapse" id="navbar_collapse_1">
		    <!-- меню на обычных/маленьких устройствах-->
		    <div class="col-md-10 col-lg-10 col-sm-10 col-xs-10 my_menu">
		      <ul id="nav" class="nav navbar-nav navbar-right ">
		        <li class=""><a href="#about">Stream</a></li>
		        <li class=""><a href="#contact">Members</a></li>
		        <li class=""><a href="#projects">Teams</a></li>
		        <li class=""><a href="#blog">Skills</a></li>  
		        <li class=""><a href="#">Stats</a></li>
		        <li class=""><a href="#">Me</a></li>
		        <li class=""><a href="#">Options</a></li>
		        <li class=""><a href="#">Invite</a></li>
		      </ul>
		      </div>
		    </div>
		  </div>              
		</nav>
	</div>
	<!--модальное окно играет роль сайдбара. это первый сайдбар, который выскакивает при нажатии кнопки login в области панели навигации-->         
          <div class="modal fade" id="modal-sidebar-login">
            <div class="modal-dialog">
              <div class="modal-content">
                <button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
                <div class="modal-header">          
                  <h4 class="title col-md-12 col-sm-12 col-xs-12 col-lg-12">Login</h4>        
                </div>
                <div class="modal-body">
                  <input id="left-line-red" class="text col-md-12 col-sm-12 col-xs-12 col-lg-12" type="wrong_pass" placeholder="Wrong password">
                  <div id="left-line-blue" class="input-group input-group-md col-md-12 col-sm-12 col-xs-12 col-lg-12">      
                    <span id="inp-gr-login" class="input-group-addon"><img src="../assets/User-96.png" alt="logo of a user"></span>
                    <input id="loginbox" type="loginbox" placeholder="Login">
                  </div>
                  <br>        
                  <div id="left-line-red" class="input-group input-group-md col-md-12 col-sm-12 col-xs-12 col-lg-12">
                    <span id="inp-gr-pass" class="input-group-addon"><img src="../assets/Key-96.png" alt="logo of a user"></span>
                    <input id="passinbox" type="passinbox" placeholder="Password">
                  </div>
                  <button type="submit" class="login1 col-md-12 col-sm-12 col-xs-12 col-lg-12">login</button>
                  <br>                
                  <button class="col-md-10 col-sm-10 col-xs-10 col-lg-10 " id="forgot_pass"><a href="#recover_pass">Forgot password</a></button>
                </div>                    
              </div>
            </div>
          </div>
	 
	</div> 
</template>

<script>
export default {
	name: 'app-header',
	data () {
		return {

		}
	},
	methods: {
		open_loginform: function(){
			$('#modal-sidebar-login').modal();
		}
	}  	
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
@import (less)  '../../../less/style.less';

</style>