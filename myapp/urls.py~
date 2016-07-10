from django.conf.urls import patterns, include, url
from django.contrib import admin
from login.views import *
 
urlpatterns = patterns('',
   # url(r'^polls/', home),
    url(r'^admin/', include(admin.site.urls)),
    url(r'^$', 'django.contrib.auth.views.login'),
    url(r'^polls/', include('polls.urls', namespace="polls")),
    url(r'^logout/$', logout_page),
    url(r'^accounts/login/$', 'django.contrib.auth.views.login'), # If user is not login it will redirect to login page
    url(r'^register/$', register),
    url(r'^register/success/$', register_success),
    url(r'^home/$', home),
    url(r'^accounts/', include('django.contrib.auth.urls')),
)
