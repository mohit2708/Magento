# Install Magento Using CMD

### Step1:
1. create folder in xammp/htdocs/magento_training
2. open cmd in this dirctery
3. __D:\xampp7.3\htdocs\mohit\magento_training>__ composer create-project --repository-url=https://repo.magento.com/ magento/project-community-edition=2.3.5-p2 (install-directory-name)

# Issues:
### icon not showing
1. Go to pub/static directory and remove everything except the .htaccess file
2. Open up app/etc/di.xml find the path
```php
Magento\Framework\App\View\Asset\MaterializationStrategy\Symlink
and replace it with
Magento\Framework\App\View\Asset\MaterializationStrategy\Copy
```
3. ki


# Install Magento
1. Download magento folder -> https://magento.com/tech-resources/download
2. and unzip folder in __xampp/htdocs__ folder 
3. 


