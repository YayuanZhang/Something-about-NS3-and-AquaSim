**Step 1 Importing project**

**Step 2 Configuring project**

   Click Projects on the left.
   
   **Under Build Settings**
   
   Remove “make all” under **Build** Steps, and click Add Build Step->Custom Process Step  
                
   > Command: should be "./waf"
   > Command arguments: "build"   
   > Working directory: default  
                
                    
   Remove “make clean” under **Clean** Steps, and click Add Clean Step->Custom Process Step  
                          
   > Command: should be "./waf"                              
   > Command arguments: "clean"                
   > Working directory: default 
                
    
  **Under Run Settings**
     
   > Executable:  "./build/examples/tutorial/ns3-dev-first-debug" or any executable you want to run and debug
     
   If you set it to "./build/examples/tutorial/ns3-dev-first-debug" make sure you used "--enable-examples" option in "./waf configure" prior to running the code     
     
   > Command arguments: blank                    
   > Working directory: default
     
   
[reference](https://www.nsnam.org/wiki/HOWTO_configure_QtCreator_with_ns-3/) **chaining QtCreator to waf**  

