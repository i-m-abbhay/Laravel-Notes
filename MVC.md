> It states that whenever we need to reed something we are not directly tell that I need something. We tell the controller to get the data it's controller's responsibility to fetch the data and pass the views back to us.

![[Pasted image 20230715081743.png]]

## View
> It's the html part which represents the current model state. for example the blade file of mvc pattern.


## Controller
> Controls and decides the data flow.
> Every controller extends the Base Controller of Laravel
> _Make sure that controller is always lean, minimal and very very Short. Should not include any logic of your application_


## Model
> Models help us to interact with the database.
> This is responsible to do all the CRUD mySQL query in a particular table.
> _if any class extends Model class of Laravel then that class becomes a model_  

**Laravel provides a convention whatever the name of the model file the plural of that will be the name of the table. But you can explicitly define your table name by following the below code in your Model class inside the model file that you're working with:**

```php

<?php

  

namespace App\Models;

  

use Illuminate\Database\Eloquent\Model;

  

class Book extends Model

{

  protected $table = 'my_books'; 
  //The model will now use my_books table instead of books by default.

}

```