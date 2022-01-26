**Note :** to work with media `pillow` must be installed in your system.
- go to settings.py and write `MEDIA_ROOT = os.path.join(BASE_DIR,"media")`
- and `MEDIA_URL = "/media/"`

- edit urls.py of project like this
```
......
from django.conf import settings
from django.conf.urls.static import static
from . import views

urlpatterns = [the
    path('admin/', admin.site.urls),
    path('', views.index,name='Home'),
    path('blog/', include("blog.urls")),
    path('shop/', include("shop.urls")),

] + static(settings.MEDIA_URL,document_root=settings.MEDIA_ROOT)

```
