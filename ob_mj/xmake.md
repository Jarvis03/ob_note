add_rules("mode.debug", "mode.release")  
  
target("test_trans")  
   set_kind("static")  
   add_files("trans_file.c")  
   add_files("cli.c")  
   add_files("aging_mode.c")  
   add_files("crc.c")  
   add_files("test_sprintf.c")  
      
target("main")  
   set_kind("binary")  
   add_files("main.c")  
  
   add_deps("test_trans")  
   add_syslinks("pthread")  
