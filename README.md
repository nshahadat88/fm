# simple-php-mvc-framework-oscar

-- Make Controller: File name & class name must be same example: index_fmc.php and it class name Index_Fmc 

-- View Load in controller
  -- $this->Load_View(pagename);
  or
  -- $view = new View();
     $view->Assign("title", "Add");
     $view->Render("directory(ifany)".DS."pagename");
 
-- load CSS file
  -- $this->view->Set_CSS('public' . DS . 'css' . DS . 'style.css');
  
-- Set page title
  -- $this->view->Set_Site_Title( "FM MVC" );
  
-- HEADER
  -- $header = new View();
		$header->Assign('app_title', "MVC Calculator App Demo");
		$this->Assign('header', $header->Render('header', false));
		
-- Footer
  -- $footer = new View();
		$this->Assign('footer', $footer->Render('footer', false));
		
-- 
