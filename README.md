# Install Magento Using CMD

### Requirments
1. install composer  https://getcomposer.org/download/

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
### admin black Screen
Go to /vendor/magento/framework/View/Element/Template/File/Validator.php<br>
$realPath = $this->fileDriver->getRealPath($path); __repalce to__ $realPath = str_replace('\\', '/', $this->fileDriver->getRealPath($path));

### Clear Cache in Magento 2
Go to System > Tools > Cache Management.

# Install Magento
1. Download magento folder -> https://magento.com/tech-resources/download
2. and unzip folder in __xampp/htdocs__ folder 
3. 

### Category
Go to admin->catalog->categories<br>
Two Types of category<br>
1. Add Root Category:- mutipal store ke liye root category banate hai
2. Add Subcategory:- single category ke liye sub category

### Product
Go to admin->catalog->Products<br>
1. Simple Product
2. Configurable Product
3. Virtual Product
4. Grouped Product
5. Bundle Product
6. Downloadable Product

### Product Attributes
Go to admin->stores->Attributes(Product)<br>
ex:- colour, size, ml


