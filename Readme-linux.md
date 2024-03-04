## Linux cheat sheet

1. Display information about the operating system distribution

    ```bash
    cat /etc/os-release
    ```
   
2. Edit filename starting at line 1

    ```bash
    vi filename	 
    ```
   
3. **i** - insert text before cursor, until <Esc> hit
4. **:wq<Return>** - quit vi, writing out modified file to file named in original invocation

5. Start Nginx service

    ```bash
    sudo service nginx start	 
    ```

6. Check Nginx service status

    ```bash
    sudo service nginx status	
    ```