<?php
defined('BASEPATH') OR exit('no direct script access allowed');

class Welcome extends CI_controller {
	
	public function index()

	$this->load->view('index');
}
public function admin_master()
  {
    $this->form_validation->set_rules('id','id','required|trim');
    $this->form_validation->set_rules('name','username','required|trim');
    $this->form_validation->set_rules('password','password','required|trim');
    }
   
   if($this->form_validation->run()==true)
   {
   $this->load->model('Demo_model');
   $this->Demo->model('insert_data();
   }
   {
        $this->index();

   }
 }


//  controller coding
<?php
class Demo_model extends CI_Model
{
	public function insert_data()
	{
	$data = array('id' => $this->input->('id');
                'name' => $this->input->('name');
	              'password => $this->input->password'
	              'id' => $this->input->('id');


	              $this->insert('admin_master','$data');
	              }
	}
}

//CATEGORY MASTER
<?php
defined('BASEPATH') OR exit('no direct script access allowed');

class Welcome extends CI_controller {
	
	public function index()

	$this->load->view('category_master');
}
public function checking()
  {
  $this->form_validation->set_rules('id','id','required|trim');
    $this->form_validation->set_rules('category_name','name','required|trim');
   
    }
   
   if($this->form_validation->run()==true)
   {
   $this->load->model('Demo_model');
   $this->Demo->model('insert_data();
   }
   {
        $this->category_master();

   }
 }
//conttroller
<?php
class Demo_model extends CI_Model
{
	public function insert_data()
	{
	$data = array('id' => $this->input->('id');
                  'category_name' => $this->input->('name');
	              


	              $this->insert(category_master','$data');
	              }
	}
}
// product_master
<?php
class user extends CI_Controller
{
	public function insert_data()
	{
	  return view('admin_master','category_master');
	}
	public function insert_data()
	{
	$data = ['id'=>$this->request->getvar('id'),
	        category_id=>this->request->getvar('category_id'),
	        product_title=>this->request->product_title('product_title'),
             prdouct_sku=>this->request->getvar('productsku'),
             product_price=>this->request->getvar('product_price'),
             //$db = \configg\Database:: connect();
             $builder = $db->table()
             $builder = $db($data);





	         ]
	}
}
<?
