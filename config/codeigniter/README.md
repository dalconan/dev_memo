# Codeigniter
## 移除index.php
### Apache
1. 在根目錄加入.htaccess檔案，內容如下
    ```
    <IfModule mod_rewrite.c>
        RewriteEngine on
        RewriteBase /
        # Hide the app directories by redirecting the request to index.php
        RewriteRule ^(app|\.svn) index.php/$1 [L]
        RewriteCond %{REQUEST_FILENAME} !-f
        RewriteCond %{REQUEST_FILENAME} !-d
        RewriteRule ^(.*)$ index.php/$1 [QSA,L]
    </IfModule>
    ```
    注意必須安裝urlrewirte功能

2. 開啟app/config/config.php修改
    ```
    $config['index_page'] = '';
    ```

3. httpd.conf中的AllowOverride None要改為  
    ```
    AllowOverride All 
    ```

4. 重新啟動apache
