**Commands :**
- C1 `python manage.py shell`

**Example :**
```
>>> from shop.models import product

>>> from django.utils import timezone                 

>>> myprod1 = product(product_name="product 2",category = "cat 2",sub_category = "sub cat 2", price = 1088, desc = "this is a good product")

>>>myprod1.save()

>>> product.objects.get(product_name = "product 1")
<product: 1- product 1>


```
