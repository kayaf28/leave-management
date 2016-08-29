# leave-management
<html>
<head>
<title>Insert Data Into Database Using CodeIgniter Form</title>
 <meta charset = "utf-8"> 
      <title>INSERT NEW EMPLOYEE</title> 
      <link rel = "stylesheet" type = "text/css" 
      href = "<?php echo $this->config->item('base_url');?>css/style.css">
      <link rel = "stylesheet" type = "text/css" 
      href = "<?php echo $this->config->item('base_url');?>css/bootstrap.css">
      <link rel = "stylesheet" type = "text/css" 
      href = "<?php echo $this->config->item('base_url');?>css/bootstrap.min.css">
      <link rel = "stylesheet" type = "text/css" 
      href = "<?php echo $this->config->item('base_url');?>css/font-awesome.css">
      <link rel = "stylesheet" type = "text/css" 
      href = "<?php echo $this->config->item('base_url');?>css/font-awesome.min.css">
      <script type='text/javascript' src="<?php echo $this->config->item('base_url'); ?>js/bootstrap.min.js"></script>
      <script type='text/javascript' src="<?php echo $this->config->item('base_url'); ?>js/jquery-1.11.0.js"></script>
      <script type='text/javascript' src="<?php echo $this->config->item('base_url'); ?>js/bootstrap.js"></script>
</head>
<body>

<div class="container-fluid">
    <div class="row">
    	<div class=" col-sm-5">
	        <?php echo form_open('insert_ctrl'); ?>
	          <h1 class="text-center login-title">Insert New EMployee into database</h1><hr/>
        <?php if (isset($message))
         { ?>

            <CENTER><h3 style="color:green;">Data inserted successfully</h3></CENTER><br>
           <?php } ?>
          <?php echo form_label('Employee code :'); ?> <?php echo form_error('emp_code'); ?><br />
          <?php echo form_input(array('id' => 'emp_code', 'name' => 'emp_code')); ?><br />

          <?php echo form_label('English Name :'); ?> <?php echo form_error('eng_name'); ?><br />
          <?php echo form_input(array('id' => 'eng_name', 'name' => 'eng_name')); ?><br />

          <?php echo form_label('Chinese Name :'); ?> <?php echo form_error('ch_name'); ?><br />
          <?php echo form_input(array('id' => 'ch_name', 'name' => 'ch_name')); ?><br />

          <?php echo form_label('email :'); ?> <?php echo form_error('email'); ?><br />
          <?php echo form_input(array('id' => 'email', 'name' => 'email')); ?><br />

          <?php echo form_label('password :'); ?> <?php echo form_error('passwords'); ?><br />
          <?php echo form_input(array('id' => 'password', 'name' => 'password')); ?><br />

          <?php echo form_label('Employee_type :'); ?> <?php echo form_error('emp_type'); ?><br />
          <?php echo form_input(array('id' => 'emp_type', 'name' => 'emp_type')); ?><br />

          <?php echo form_submit(array('id' => 'submit', 'value' => 'Submit')); ?>
          <?php echo form_close(); ?><br/>

          <div id="fugo">

			</div>
		</div>
	</div>
</div>
</body>
</html>
