# Comparing `tmp/cradmin_legacy-5.0.0.tar.gz` & `tmp/cradmin_legacy-5.0.0b0.tar.gz`

## Comparing `cradmin_legacy-5.0.0.tar` & `cradmin_legacy-5.0.0b0.tar`

### file list

```diff
@@ -1,631 +1,631 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/__init__.py
--rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/automodelform.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/context_processors.py
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/cradmin_testhelpers.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/crapp.py
--rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/crinstance.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/crispylayouts.py
--rw-r--r--   0        0        0     9083 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/crmenu.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/crsettings.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/css_icon_map.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/datetimeutils.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/decorators.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/delay_middleware.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/messages_debug_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/models.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/python2_compatibility.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/registry.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/renderable.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/urlutils.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/version.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/acemarkdown/__init__.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/acemarkdown/widgets.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_account/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_account/views/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/urls.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/utils.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/activate.django.html
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/email/html_message.django.html
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/email/subject.django.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/messages/activation-link-expired.django.html
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/messages/activation-link-invalid.django.html
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/messages/success.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/tests/__init__.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/tests/test_activate.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/views/__init__.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/views/activate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/__init__.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/backends.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/urls.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/templates/cradmin_authenticate/login.django.html
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/templates/cradmin_authenticate/logout.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/__init__.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/test_email_auth_backend.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/test_login.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/cradmin_authenticate_testapp/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/cradmin_authenticate_testapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/views/__init__.py
--rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/views/login.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/views/logout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/__init__.py
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/emailutils.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/management/commands/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/management/commands/ievv_email_send_testmail.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/html_message_base.django.html
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/cradmin_email_send_testmail/html_message.django.html
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/cradmin_email_send_testmail/subject.django.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/include/html_message_footer.django.html
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/include/html_message_header.django.html
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/templatetags/cradmin_email_buttonlink.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templatetags/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templatetags/cradmin_legacy_email_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/__init__.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/test_emailutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/models.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/templates/cradmin_email_testapp/abstractemail/html_message.django.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/templates/cradmin_email_testapp/abstractemail/plaintext_message.django.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/templates/cradmin_email_testapp/abstractemail/subject.django.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/views/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/views/email_design.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/admin.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/apps.py
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/cradminviews.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/models.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0001_initial.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0002_archiveimage_file_size.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0003_auto_20151017_0139.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/tests/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/tests/helpers.py
--rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/tests/test_cradminviews.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/__init__.py
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/invite_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/baseviews/__init__.py
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/baseviews/accept.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/accept.django.html
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/description.django.html
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/token_error.django.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/email/html_message.django.html
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/email/subject.django.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/tests/__init__.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/tests/test_accept.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/tests/test_invite_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/__init__.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/auth_user.py
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/base.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/email.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/base.django.html
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/begin.django.html
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/email_sent.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/cradmin_register_account_testapp/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/cradmin_register_account_testapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/forms/__init__.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_auth_user.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_email.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/views/__init__.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_begin.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_email_sent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/views/__init__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/views/begin.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/views/email_sent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/models.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/urls.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/base.django.html
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/begin.django.html
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email_sent.django.html
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/reset.django.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email/html_message.django.html
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email/subject.django.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/messages/successmessage.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/__init__.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_begin.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_email_sent.py
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_reset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/views/__init__.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/views/begin.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/views/email_sent.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/views/reset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/__init__.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/admin.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/crispylayouts.py
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/models.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/urls.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/widgets.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0001_initial.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0002_temporaryfilecollection_singlemode.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0003_temporaryfilecollection_max_filesize_bytes.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0004_auto_20151017_1947.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/bulkfileupload-submit.django.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/bulkfileupload-widget.django.html
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/include/bulkfileupload.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/__init__.py
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_models.py
--rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_temporary_file_upload_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/views/__init__.py
--rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/views/temporary_file_upload_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/cradmin_legacy_testapp/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/cradmin_legacy_testapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/formfields/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/formfields/email_list.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/imageutils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/imageutils/backends/__init__.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/imageutils/backends/backendinterface.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/imageutils/backends/sorl_thumbnail.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    28488 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    17293 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    34294 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/sortable/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/sortable/admin.py
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/sortable/models.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/.gitignore
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/Gruntfile.coffee
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/bower.json
--rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/custom_vitalstyles_cli.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/package.json
--rw-r--r--   0        0        0   175479 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/yarn.lock
--rw-r--r--   0        0        0   193101 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_default/theme.css
--rw-r--r--   0        0        0   191616 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_topmenu/theme.css
--rw-r--r--   0        0        0   233971 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.js
--rw-r--r--   0        0        0   150994 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js
--rw-r--r--   0        0        0    97655 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js.map
--rw-r--r--   0        0        0   566450 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js
--rw-r--r--   0        0        0   544145 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js.map
--rw-r--r--   0        0        0    28747 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css
--rw-r--r--   0        0        0    21778 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css.map
--rw-r--r--   0        0        0    23739 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.min.css
--rw-r--r--   0        0        0    93888 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/FontAwesome.otf
--rw-r--r--   0        0        0    60767 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   313398 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   122092 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    71508 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    56780 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0    62927 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    41280 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0   358296 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/ace.js
--rw-r--r--   0        0        0    67747 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/mode-markdown.js
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/theme-tomorrow.js
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/af.js
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-dz.js
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-kw.js
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ly.js
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ma.js
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-sa.js
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-tn.js
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar.js
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/az.js
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/be.js
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bg.js
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bm.js
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bn.js
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bo.js
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/br.js
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bs.js
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ca.js
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cs.js
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cv.js
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cy.js
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/da.js
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-at.js
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-ch.js
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de.js
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/dv.js
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/el.js
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-au.js
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ca.js
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-gb.js
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ie.js
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-il.js
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-nz.js
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eo.js
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-do.js
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-us.js
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es.js
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/et.js
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eu.js
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fa.js
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fi.js
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fo.js
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ca.js
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ch.js
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr.js
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fy.js
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gd.js
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gl.js
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gom-latn.js
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gu.js
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/he.js
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hi.js
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hr.js
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hu.js
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hy-am.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/id.js
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/is.js
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/it.js
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ja.js
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/jv.js
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ka.js
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kk.js
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/km.js
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kn.js
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ko.js
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ky.js
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lb.js
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lo.js
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lt.js
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lv.js
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/me.js
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mi.js
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mk.js
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ml.js
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mr.js
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms-my.js
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms.js
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mt.js
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/my.js
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nb.js
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ne.js
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl-be.js
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl.js
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nn.js
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pa-in.js
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pl.js
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt-br.js
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt.js
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ro.js
--rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ru.js
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sd.js
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/se.js
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/si.js
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sk.js
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sl.js
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sq.js
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr-cyrl.js
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr.js
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ss.js
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sv.js
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sw.js
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ta.js
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/te.js
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tet.js
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tg.js
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/th.js
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tl-ph.js
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tlh.js
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tr.js
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzl.js
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm-latn.js
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm.js
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ug-cn.js
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uk.js
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ur.js
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz-latn.js
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz.js
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/vi.js
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/x-pseudo.js
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/yo.js
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-cn.js
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-hk.js
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-tw.js
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/examples/acemarkdown.html
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/acemarkdown.less
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/alerts.less
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/all.less
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bootstrap.less
--rw-r--r--   0        0        0    11010 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bulkfileupload.less
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/buttons.less
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/cradmin_authenticate.less
--rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/datetimeselector.less
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/filewidgets.less
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/focusedpage.less
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/forms.less
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/grid.less
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/icons.less
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/iframe.less
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/loadmorepager.less
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/menu.less
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/messages.less
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/mixins.less
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/modal.less
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/modelchoicefield.less
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/objecttableview.less
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/page-header.less
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/pager.less
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/roleselect.less
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/scaffolding.less
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/submitrow.less
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/table.less
--rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/variables.less
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemframe.less
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemvalue.less
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/lists.less
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/lists.less
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/target.less
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/selectableitem.less
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/target.less
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/view.less
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/menu.less
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/theme.less
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/variables.less
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_topmenu/menu.less
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_topmenu/theme.less
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_topmenu/variables.less
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/detectizr.coffee
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/iosaddtohomescreen.coffee
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/lib.coffee
--rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/acemarkdown/acemarkdown.coffee
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/acemarkdown/acemarkdown.tpl.html
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/directives.coffee
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/providers.coffee
--rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.coffee
--rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.spec.coffee
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/fileinfo.tpl.html
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/progress.tpl.html
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/rejectedfiles.tpl.html
--rw-r--r--   0        0        0    16771 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/calendar/providers.coffee
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/collapse/collapse.coffee
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/common/directives.coffee
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/common/providers.coffee
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/clearabletextinput.coffee
--rw-r--r--   0        0        0    15222 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/dateselector.tpl.html
--rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/datetimewidget.coffee
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/filewidget.coffee
--rw-r--r--   0        0        0    11146 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/modelchoicefield.coffee
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/select.coffee
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/setfieldvalue.coffee
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/usethisbutton.coffee
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.coffee
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.spec.coffee
--rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/listfilter/directives.coffee
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/directives.coffee
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/services.coffee
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/menu/menu.coffee
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/messages/controllers.coffee
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/modal/directives.coffee
--rw-r--r--   0        0        0    11288 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/directives.coffee
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/services.coffee
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/objecttable/objecttable.coffee
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/navbar.tpl.html
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/pagepreview.coffee
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/scrollfixed/directives.coffee
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/wysihtml/wysihtml.coffee
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/README.md
--rwxr-xr-x   0        0        0    36947 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.flash.swf
--rwxr-xr-x   0        0        0    42869 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.min.js
--rwxr-xr-x   0        0        0    27436 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.js
--rwxr-xr-x   0        0        0    15302 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.min.js
--rwxr-xr-x   0        0        0    12212 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.js
--rwxr-xr-x   0        0        0     7559 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.min.js
--rwxr-xr-x   0        0        0    15223 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.js
--rwxr-xr-x   0        0        0     7757 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.min.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/__init__.py
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/superuserui_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/crapps/__init__.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/crapps/djangoapp.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/crapps/djangomodel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/__init__.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/appdashboardview.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/createview.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/dashboardview.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/deleteview.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/editview.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/listview.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/mixins.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/base-internal.django.html
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/base.django.html
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/error.django.html
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/invalid_roleid.django.html
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/menu.django.html
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/menuitem.django.html
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/missing_role.django.html
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/roleselect.django.html
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/standalone-base-internal.django.html
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/standalone-base.django.html
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/acemarkdown/widget.django.html
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/apps/cradmin_imagearchive/listview.django.html
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/apps/cradmin_imagearchive/preview.django.html
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/collapsed-section-layout.django.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/cradmin_form_helper.django.html
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/submitbutton.django.html
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/filewidgets/filewidget.django.html
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/filewidgets/imagewidget.django.html
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/imageutils/templatetags/archiveimage-tag.django.html
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/include/messages.django.html
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/layouts/README.md
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused-internal.django.html
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused.django.html
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/superuserui/appdashboard.django.html
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/superuserui/dashboard.django.html
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/superuserui/listbuilder/itemvalue-djangoapp.django.html
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/superuserui/listbuilder/itemvalue-model.django.html
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/create.django.html
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/create_update_base.django.html
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/delete.django.html
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/formview_base.django.html
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/update.django.html
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/loadmorepager-base.django.html
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/pager.django.html
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/base/itemframe.django.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/base/itemvalue.django.html
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/base/list.django.html
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemframe/link.django.html
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete-with-archive-image.django.html
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete.django.html
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/titledescription.django.html
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/use-this.django.html
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/default.django.html
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-left.django.html
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-right.django.html
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-top.django.html
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/includes/create-button.django.html
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/includes/loadmorepager.django.html
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.django.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/base/filterlist.django.html
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox/base.django.html
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/radio/base.django.html
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/select/base.django.html
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/textinput/base.django.html
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect/formview.django.html
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues/itemvalue.django.html
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/preview-list.django.html
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/preview-value.django.html
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/widget.django.html
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer/selected-item.django.html
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/target_renderer/target.django.html
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/base.django.html
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/listbuilderfilterview.django.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/listbuilderview.django.html
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/button.django.html
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/imagepreviewcolumn-cell.django.html
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/multiactioncolumn-cell.django.html
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/no-items-message.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/no-searchresults-message.django.html
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-left.django.html
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-right.django.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-top.django.html
--rw-r--r--   0        0        0    13586 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/plaintextcolumn-cell.django.html
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/singleactioncolumn-cell.django.html
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/singlebuttoncolumn-cell.django.html
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/usethisactioncolumn-cell.django.html
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/includes/loadmorepager.django.html
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/widgets/datetimepicker.django.html
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/widgets/modelchoice.django.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/widgets/timepicker.django.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/wysihtml5/textareawrap.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templatetags/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templatetags/cradmin_legacy_icon_tags.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templatetags/cradmin_legacy_image_tags.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/templatetags/cradmin_legacy_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/helpers.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/test_abstract_renderable.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/test_urlutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/formfields/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/formfields/test_email_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/sortable/__init__.py
--rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/sortable/test_sortable.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/sortable/cradmin_sortable_testapp/__init__.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/sortable/cradmin_sortable_testapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/test_automodelform/__init__.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/test_automodelform/test_automodelform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/test_automodelform/cradmin_automodelform_testapp/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/test_automodelform/cradmin_automodelform_testapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/utils/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/utils/test_crhumanize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_delete.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilderview.py
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect.py
--rw-r--r--   0        0        0    24986 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_objecttable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/__init__.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/models.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/templates/cradmin_viewhelpers_testapp/listbuilder/minimal-renderable.django.html
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/templates/cradmin_viewhelpers_testapp/listfilter/minimal-filtergroupchild.django.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilder/__init__.py
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_base.py
--rw-r--r--   0        0        0    12039 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_itemvalue.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/__init__.py
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilter.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilterlist.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_filtershandler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/multi/__init__.py
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/multi/test_abstractcheckbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractradio.py
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractselect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/__init__.py
--rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_select.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_textinput.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/__init__.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_listbuilder_itemvalues.py
--rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanyview.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanywidget.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_selected_item_renderer.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_target_renderer.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_widget_preview_renderer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/views/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/views/helpers.py
--rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/tests/views/test_roleselect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/utils/__init__.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/utils/crhumanize.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/utils/nulls_last_queryset.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/__init__.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/create.py
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/crudbase.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/delete.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/detail.py
--rw-r--r--   0        0        0    16861 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/formbase.py
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilderview.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/mixins.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect.py
--rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2view.py
--rw-r--r--   0        0        0    52172 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/objecttable.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/update.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/__init__.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/base.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/itemframe.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/itemvalue.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/lists.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/__init__.py
--rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/listfilter_viewmixin.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/lists.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/__init__.py
--rw-r--r--   0        0        0    10684 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.py
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlist.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlistchild.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/exceptions.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/filtershandler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/multi/__init__.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/multi/abstractcheckbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/__init__.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractradio.py
--rw-r--r--   0        0        0    17113 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractselect.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstracttextinput.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/base.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/multi/__init__.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/single/__init__.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/single/select.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/single/textinput.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/__init__.py
--rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues.py
--rw-r--r--   0        0        0     8468 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/manytomanyview.py
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer.py
--rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/target_renderer.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/widget_preview_renderer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/views/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/views/roleselect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/widgets/__init__.py
--rw-r--r--   0        0        0    38041 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/widgets/datetimepicker.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/widgets/filewidgets.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/widgets/modelchoice.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/widgets/selectwidgets.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/wysihtml5/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/cradmin_legacy/wysihtml5/widgets.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/.gitignore
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/LICENSE
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/README.md
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/__init__.py
+-rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/automodelform.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/context_processors.py
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/cradmin_testhelpers.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/crapp.py
+-rw-r--r--   0        0        0    15872 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/crinstance.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/crispylayouts.py
+-rw-r--r--   0        0        0     9083 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/crmenu.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/crsettings.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/css_icon_map.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/datetimeutils.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/decorators.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/delay_middleware.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/messages_debug_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/models.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/python2_compatibility.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/registry.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/renderable.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/urlutils.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/version.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/acemarkdown/__init__.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/acemarkdown/widgets.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_account/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_account/views/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/urls.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/utils.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/activate.django.html
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/email/html_message.django.html
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/email/subject.django.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/messages/activation-link-expired.django.html
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/messages/activation-link-invalid.django.html
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/messages/success.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/tests/__init__.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/tests/test_activate.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/views/__init__.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/views/activate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/__init__.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/backends.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/urls.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/templates/cradmin_authenticate/login.django.html
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/templates/cradmin_authenticate/logout.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/__init__.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/test_email_auth_backend.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/test_login.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/cradmin_authenticate_testapp/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/cradmin_authenticate_testapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/views/__init__.py
+-rw-r--r--   0        0        0    10717 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/views/login.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/views/logout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/__init__.py
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/emailutils.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/management/commands/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/management/commands/ievv_email_send_testmail.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/html_message_base.django.html
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/cradmin_email_send_testmail/html_message.django.html
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/cradmin_email_send_testmail/subject.django.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/include/html_message_footer.django.html
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/include/html_message_header.django.html
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/templatetags/cradmin_email_buttonlink.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templatetags/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templatetags/cradmin_legacy_email_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/__init__.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/test_emailutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/models.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/templates/cradmin_email_testapp/abstractemail/html_message.django.html
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/templates/cradmin_email_testapp/abstractemail/plaintext_message.django.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/cradmin_email_testapp/templates/cradmin_email_testapp/abstractemail/subject.django.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/views/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/views/email_design.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/admin.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/apps.py
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/cradminviews.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/models.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0001_initial.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0002_archiveimage_file_size.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0003_auto_20151017_0139.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/tests/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/tests/helpers.py
+-rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/tests/test_cradminviews.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/__init__.py
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/invite_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/baseviews/__init__.py
+-rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/baseviews/accept.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/accept.django.html
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/description.django.html
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/token_error.django.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/email/html_message.django.html
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/email/subject.django.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/tests/__init__.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/tests/test_accept.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/tests/test_invite_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/__init__.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/auth_user.py
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/base.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/email.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/base.django.html
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/begin.django.html
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/email_sent.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/cradmin_register_account_testapp/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/cradmin_register_account_testapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/forms/__init__.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_auth_user.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_email.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/views/__init__.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_begin.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_email_sent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/views/__init__.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/views/begin.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/views/email_sent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/models.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/urls.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/base.django.html
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/begin.django.html
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email_sent.django.html
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/reset.django.html
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email/html_message.django.html
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email/subject.django.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/messages/successmessage.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/__init__.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_begin.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_email_sent.py
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_reset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/views/__init__.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/views/begin.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/views/email_sent.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/views/reset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/__init__.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/admin.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/crispylayouts.py
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/models.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/urls.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/widgets.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0001_initial.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0002_temporaryfilecollection_singlemode.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0003_temporaryfilecollection_max_filesize_bytes.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0004_auto_20151017_1947.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/bulkfileupload-submit.django.html
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/bulkfileupload-widget.django.html
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/include/bulkfileupload.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/__init__.py
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_models.py
+-rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_temporary_file_upload_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/views/__init__.py
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/views/temporary_file_upload_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/cradmin_legacy_testapp/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/cradmin_legacy_testapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/formfields/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/formfields/email_list.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/backends/__init__.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/backends/backendinterface.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/backends/sorl_thumbnail.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    28488 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17293 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    34294 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/sortable/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/sortable/admin.py
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/sortable/models.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/.gitignore
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/Gruntfile.coffee
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/bower.json
+-rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/custom_vitalstyles_cli.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/package.json
+-rw-r--r--   0        0        0   175479 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/yarn.lock
+-rw-r--r--   0        0        0   193101 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_default/theme.css
+-rw-r--r--   0        0        0   191616 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_topmenu/theme.css
+-rw-r--r--   0        0        0   233971 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.js
+-rw-r--r--   0        0        0   150994 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js
+-rw-r--r--   0        0        0    97655 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js.map
+-rw-r--r--   0        0        0   566450 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js
+-rw-r--r--   0        0        0   544145 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js.map
+-rw-r--r--   0        0        0    28747 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css
+-rw-r--r--   0        0        0    21778 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css.map
+-rw-r--r--   0        0        0    23739 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.min.css
+-rw-r--r--   0        0        0    93888 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0    60767 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   313398 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   122092 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    71508 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    56780 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0    62927 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    41280 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0   358296 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/ace.js
+-rw-r--r--   0        0        0    67747 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/mode-markdown.js
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/theme-tomorrow.js
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/af.js
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-dz.js
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-kw.js
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ly.js
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ma.js
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-sa.js
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-tn.js
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar.js
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/az.js
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/be.js
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bg.js
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bm.js
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bn.js
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bo.js
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/br.js
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bs.js
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ca.js
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cs.js
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cv.js
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cy.js
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/da.js
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-at.js
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-ch.js
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de.js
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/dv.js
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/el.js
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-au.js
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ca.js
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-gb.js
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ie.js
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-il.js
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-nz.js
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eo.js
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-do.js
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-us.js
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es.js
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/et.js
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eu.js
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fa.js
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fi.js
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fo.js
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ca.js
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ch.js
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr.js
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fy.js
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gd.js
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gl.js
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gom-latn.js
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gu.js
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/he.js
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hi.js
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hr.js
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hu.js
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hy-am.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/id.js
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/is.js
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/it.js
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ja.js
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/jv.js
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ka.js
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kk.js
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/km.js
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kn.js
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ko.js
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ky.js
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lb.js
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lo.js
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lt.js
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lv.js
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/me.js
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mi.js
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mk.js
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ml.js
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mr.js
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms-my.js
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms.js
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mt.js
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/my.js
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nb.js
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ne.js
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl-be.js
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl.js
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nn.js
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pa-in.js
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pl.js
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt-br.js
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt.js
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ro.js
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ru.js
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sd.js
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/se.js
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/si.js
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sk.js
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sl.js
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sq.js
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr-cyrl.js
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr.js
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ss.js
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sv.js
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sw.js
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ta.js
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/te.js
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tet.js
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tg.js
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/th.js
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tl-ph.js
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tlh.js
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tr.js
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzl.js
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm-latn.js
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm.js
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ug-cn.js
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uk.js
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ur.js
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz-latn.js
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz.js
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/vi.js
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/x-pseudo.js
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/yo.js
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-cn.js
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-hk.js
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-tw.js
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/examples/acemarkdown.html
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/acemarkdown.less
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/alerts.less
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/all.less
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bootstrap.less
+-rw-r--r--   0        0        0    11010 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bulkfileupload.less
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/buttons.less
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/cradmin_authenticate.less
+-rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/datetimeselector.less
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/filewidgets.less
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/focusedpage.less
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/forms.less
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/grid.less
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/icons.less
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/iframe.less
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/loadmorepager.less
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/menu.less
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/messages.less
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/mixins.less
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/modal.less
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/modelchoicefield.less
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/objecttableview.less
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/page-header.less
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/pager.less
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/roleselect.less
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/scaffolding.less
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/submitrow.less
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/table.less
+-rw-r--r--   0        0        0    14745 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/variables.less
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemframe.less
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemvalue.less
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/lists.less
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/lists.less
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/target.less
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/selectableitem.less
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/target.less
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/view.less
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/menu.less
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/theme.less
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/variables.less
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_topmenu/menu.less
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_topmenu/theme.less
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_topmenu/variables.less
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/detectizr.coffee
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/iosaddtohomescreen.coffee
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/lib.coffee
+-rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/acemarkdown/acemarkdown.coffee
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/acemarkdown/acemarkdown.tpl.html
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/directives.coffee
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/providers.coffee
+-rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.coffee
+-rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.spec.coffee
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/fileinfo.tpl.html
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/progress.tpl.html
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/rejectedfiles.tpl.html
+-rw-r--r--   0        0        0    16771 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/calendar/providers.coffee
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/collapse/collapse.coffee
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/common/directives.coffee
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/common/providers.coffee
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/clearabletextinput.coffee
+-rw-r--r--   0        0        0    15222 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/dateselector.tpl.html
+-rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/datetimewidget.coffee
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/filewidget.coffee
+-rw-r--r--   0        0        0    11146 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/modelchoicefield.coffee
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/select.coffee
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/setfieldvalue.coffee
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/usethisbutton.coffee
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.coffee
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.spec.coffee
+-rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/listfilter/directives.coffee
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/directives.coffee
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/services.coffee
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/menu/menu.coffee
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/messages/controllers.coffee
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/modal/directives.coffee
+-rw-r--r--   0        0        0    11288 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/directives.coffee
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/services.coffee
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/objecttable/objecttable.coffee
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/navbar.tpl.html
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/pagepreview.coffee
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/scrollfixed/directives.coffee
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/wysihtml/wysihtml.coffee
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/README.md
+-rwxr-xr-x   0        0        0    36947 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.flash.swf
+-rwxr-xr-x   0        0        0    42869 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.min.js
+-rwxr-xr-x   0        0        0    27436 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.js
+-rwxr-xr-x   0        0        0    15302 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.min.js
+-rwxr-xr-x   0        0        0    12212 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.js
+-rwxr-xr-x   0        0        0     7559 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.min.js
+-rwxr-xr-x   0        0        0    15223 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.js
+-rwxr-xr-x   0        0        0     7757 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.min.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/__init__.py
+-rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/superuserui_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/crapps/__init__.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/crapps/djangoapp.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/crapps/djangomodel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/__init__.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/appdashboardview.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/createview.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/dashboardview.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/deleteview.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/editview.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/listview.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/mixins.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/base-internal.django.html
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/base.django.html
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/error.django.html
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/invalid_roleid.django.html
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/menu.django.html
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/menuitem.django.html
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/missing_role.django.html
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/roleselect.django.html
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/standalone-base-internal.django.html
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/standalone-base.django.html
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/acemarkdown/widget.django.html
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/apps/cradmin_imagearchive/listview.django.html
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/apps/cradmin_imagearchive/preview.django.html
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/collapsed-section-layout.django.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/cradmin_form_helper.django.html
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/submitbutton.django.html
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/filewidgets/filewidget.django.html
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/filewidgets/imagewidget.django.html
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/imageutils/templatetags/archiveimage-tag.django.html
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/include/messages.django.html
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/layouts/README.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused-internal.django.html
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused.django.html
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/superuserui/appdashboard.django.html
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/superuserui/dashboard.django.html
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/superuserui/listbuilder/itemvalue-djangoapp.django.html
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/superuserui/listbuilder/itemvalue-model.django.html
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/create.django.html
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/create_update_base.django.html
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/delete.django.html
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/formview_base.django.html
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/update.django.html
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/loadmorepager-base.django.html
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/pager.django.html
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/base/itemframe.django.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/base/itemvalue.django.html
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/base/list.django.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemframe/link.django.html
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete-with-archive-image.django.html
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete.django.html
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/titledescription.django.html
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/use-this.django.html
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/default.django.html
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-left.django.html
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-right.django.html
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-top.django.html
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/includes/create-button.django.html
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/includes/loadmorepager.django.html
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.django.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/base/filterlist.django.html
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox/base.django.html
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/radio/base.django.html
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/select/base.django.html
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/textinput/base.django.html
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect/formview.django.html
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues/itemvalue.django.html
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/preview-list.django.html
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/preview-value.django.html
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/widget.django.html
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer/selected-item.django.html
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/target_renderer/target.django.html
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/base.django.html
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/listbuilderfilterview.django.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/listbuilderview.django.html
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/button.django.html
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/imagepreviewcolumn-cell.django.html
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/multiactioncolumn-cell.django.html
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/no-items-message.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/no-searchresults-message.django.html
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-left.django.html
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-right.django.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-top.django.html
+-rw-r--r--   0        0        0    13586 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/plaintextcolumn-cell.django.html
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/singleactioncolumn-cell.django.html
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/singlebuttoncolumn-cell.django.html
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/usethisactioncolumn-cell.django.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/includes/loadmorepager.django.html
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/widgets/datetimepicker.django.html
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/widgets/modelchoice.django.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/widgets/timepicker.django.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/wysihtml5/textareawrap.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/cradmin_legacy_icon_tags.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/cradmin_legacy_image_tags.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/cradmin_legacy_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/helpers.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_abstract_renderable.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_urlutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/formfields/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/formfields/test_email_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/sortable/__init__.py
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/sortable/test_sortable.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/sortable/cradmin_sortable_testapp/__init__.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/sortable/cradmin_sortable_testapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_automodelform/__init__.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_automodelform/test_automodelform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_automodelform/cradmin_automodelform_testapp/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_automodelform/cradmin_automodelform_testapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/utils/test_crhumanize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_delete.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilderview.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect.py
+-rw-r--r--   0        0        0    24986 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_objecttable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/__init__.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/models.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/templates/cradmin_viewhelpers_testapp/listbuilder/minimal-renderable.django.html
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/templates/cradmin_viewhelpers_testapp/listfilter/minimal-filtergroupchild.django.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilder/__init__.py
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_base.py
+-rw-r--r--   0        0        0    12039 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_itemvalue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/__init__.py
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilter.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilterlist.py
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_filtershandler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/multi/__init__.py
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/multi/test_abstractcheckbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractradio.py
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractselect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/__init__.py
+-rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_select.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_textinput.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/__init__.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_listbuilder_itemvalues.py
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanyview.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanywidget.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_selected_item_renderer.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_target_renderer.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_widget_preview_renderer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/views/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/views/helpers.py
+-rw-r--r--   0        0        0    11410 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/tests/views/test_roleselect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/utils/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/utils/crhumanize.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/utils/nulls_last_queryset.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/__init__.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/create.py
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/crudbase.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/delete.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/detail.py
+-rw-r--r--   0        0        0    16861 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/formbase.py
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilderview.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/mixins.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect.py
+-rw-r--r--   0        0        0    16773 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2view.py
+-rw-r--r--   0        0        0    52172 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/objecttable.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/update.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/__init__.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/base.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/itemframe.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/itemvalue.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/lists.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/__init__.py
+-rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/listfilter_viewmixin.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/lists.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/__init__.py
+-rw-r--r--   0        0        0    10684 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.py
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlist.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlistchild.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/exceptions.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/filtershandler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/multi/__init__.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/multi/abstractcheckbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/__init__.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractradio.py
+-rw-r--r--   0        0        0    17113 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractselect.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstracttextinput.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/base.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/multi/__init__.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/single/__init__.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/single/select.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/single/textinput.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/__init__.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues.py
+-rw-r--r--   0        0        0     8468 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/manytomanyview.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer.py
+-rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/target_renderer.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/widget_preview_renderer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/views/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/views/roleselect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/__init__.py
+-rw-r--r--   0        0        0    38041 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/datetimepicker.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/filewidgets.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/modelchoice.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/selectwidgets.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/wysihtml5/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/cradmin_legacy/wysihtml5/widgets.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/.gitignore
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/LICENSE
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/README.md
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 cradmin_legacy-5.0.0b0/PKG-INFO
```

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/automodelform.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/automodelform.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/context_processors.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/context_processors.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/cradmin_testhelpers.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/cradmin_testhelpers.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/crapp.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/crapp.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/crinstance.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/crinstance.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/crispylayouts.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/crispylayouts.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/crmenu.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/crmenu.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/css_icon_map.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/css_icon_map.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/datetimeutils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/decorators.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/decorators.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/delay_middleware.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/delay_middleware.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/messages_debug_middleware.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/messages_debug_middleware.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/registry.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/registry.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/renderable.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/renderable.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/urlutils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/urlutils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/acemarkdown/widgets.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/acemarkdown/widgets.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/utils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/utils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/activate.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/templates/cradmin_activate_account/activate.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/tests/test_activate.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/tests/test_activate.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/tests/test_utils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_activate_account/views/activate.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_activate_account/views/activate.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/backends.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/backends.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/templates/cradmin_authenticate/login.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/templates/cradmin_authenticate/login.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/test_email_auth_backend.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/test_email_auth_backend.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/tests/test_login.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_authenticate/views/login.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_authenticate/views/login.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/emailutils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/emailutils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/management/commands/ievv_email_send_testmail.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/management/commands/ievv_email_send_testmail.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/html_message_base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/html_message_base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/cradmin_email_send_testmail/html_message.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templates/cradmin_email/cradmin_email_send_testmail/html_message.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/templatetags/cradmin_legacy_email_tags.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/templatetags/cradmin_legacy_email_tags.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/tests/test_emailutils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/tests/test_emailutils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_email/views/email_design.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_email/views/email_design.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/admin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/admin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/cradminviews.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/cradminviews.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0001_initial.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0003_auto_20151017_0139.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/migrations/0003_auto_20151017_0139.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/tests/helpers.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_imagearchive/tests/test_cradminviews.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_imagearchive/tests/test_cradminviews.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/invite_url.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/invite_url.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/baseviews/accept.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/baseviews/accept.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/accept.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/accept.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/token_error.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/templates/cradmin_invite/accept/token_error.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/tests/test_accept.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/tests/test_accept.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_invite/tests/test_invite_url.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_invite/tests/test_invite_url.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/auth_user.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/auth_user.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/base.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/base.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/forms/email.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/forms/email.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/begin.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/begin.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/email_sent.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/templates/cradmin_register_account/email_sent.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_auth_user.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_auth_user.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_email.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/forms/test_email.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_begin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_begin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_email_sent.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/tests/views/test_email_sent.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_register_account/views/begin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_register_account/views/begin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/urls.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/urls.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email_sent.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email_sent.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/reset.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/reset.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email/html_message.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/templates/cradmin_resetpassword/email/html_message.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_begin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_begin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_email_sent.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_email_sent.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_reset.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/views/begin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/views/begin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_resetpassword/views/reset.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_resetpassword/views/reset.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/admin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/admin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/crispylayouts.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/crispylayouts.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/widgets.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/widgets.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0001_initial.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0002_temporaryfilecollection_singlemode.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0002_temporaryfilecollection_singlemode.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0003_temporaryfilecollection_max_filesize_bytes.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0003_temporaryfilecollection_max_filesize_bytes.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0004_auto_20151017_1947.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/migrations/0004_auto_20151017_1947.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/include/bulkfileupload.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/templates/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/include/bulkfileupload.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_temporary_file_upload_api.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/tests/test_temporary_file_upload_api.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/views/temporary_file_upload_api.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/apps/cradmin_temporaryfileuploadstore/views/temporary_file_upload_api.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/cradmin_legacy_testapp/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/cradmin_legacy_testapp/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/formfields/email_list.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/formfields/email_list.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/imageutils/__init__.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/imageutils/backends/backendinterface.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/backends/backendinterface.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/imageutils/backends/sorl_thumbnail.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/imageutils/backends/sorl_thumbnail.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/locale/en/LC_MESSAGES/django.po` & `cradmin_legacy-5.0.0b0/cradmin_legacy/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/locale/nb/LC_MESSAGES/django.mo` & `cradmin_legacy-5.0.0b0/cradmin_legacy/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/locale/nb/LC_MESSAGES/django.po` & `cradmin_legacy-5.0.0b0/cradmin_legacy/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/sortable/admin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/sortable/admin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/sortable/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/sortable/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/Gruntfile.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/Gruntfile.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/bower.json` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/bower.json`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/custom_vitalstyles_cli.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/custom_vitalstyles_cli.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/package.json` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/package.json`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/yarn.lock` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/yarn.lock`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_default/theme.css` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_default/theme.css`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_topmenu/theme.css` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/css/cradmin_theme_topmenu/theme.css`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js.map` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/js/cradmin.min.js.map`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js.map` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/cradmin-vendorjs.js.map`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css.map` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.min.css` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/FontAwesome.otf` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.eot` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.svg` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.ttf` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff2` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/fontawesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/fonts/glyphicons/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/ace.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/ace.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/mode-markdown.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/mode-markdown.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/theme-tomorrow.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/js/ace-editor/theme-tomorrow.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/af.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/af.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-dz.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-kw.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-kw.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ly.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ma.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-sa.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-tn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ar.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/az.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/az.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/be.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/be.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bg.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bg.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bm.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bm.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bo.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bo.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/br.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/br.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bs.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/bs.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ca.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ca.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cs.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cs.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cv.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cv.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cy.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/cy.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/da.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/da.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-at.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-at.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-ch.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de-ch.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/de.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/dv.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/dv.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/el.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/el.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-au.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-au.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ca.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-gb.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ie.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-il.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-il.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-nz.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eo.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eo.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-do.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-do.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-us.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es-us.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/es.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/et.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/et.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eu.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/eu.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fa.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fa.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fi.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fi.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fo.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fo.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ca.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ch.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fr.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fy.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/fy.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gd.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gd.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gl.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gl.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gom-latn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gom-latn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gu.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/gu.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/he.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/he.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hi.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hi.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hr.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hr.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hu.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hu.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hy-am.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/hy-am.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/id.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/id.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/is.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/is.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/it.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/it.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ja.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ja.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/jv.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/jv.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ka.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ka.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kk.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kk.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/km.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/km.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/kn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ko.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ko.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ky.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ky.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lb.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lb.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lo.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lo.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lt.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lt.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lv.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/lv.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/me.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/me.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mi.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mi.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mk.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mk.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ml.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ml.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mr.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mr.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms-my.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ms.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mt.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/mt.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/my.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/my.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nb.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nb.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ne.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ne.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl-be.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nl.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/nn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pa-in.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pa-in.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pl.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pl.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt-br.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/pt.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ro.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ro.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ru.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ru.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sd.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sd.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/se.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/se.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/si.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/si.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sk.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sk.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sl.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sl.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sq.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sq.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr-cyrl.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sr.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ss.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ss.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sv.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sv.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sw.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/sw.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ta.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ta.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/te.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/te.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tet.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tet.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tg.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tg.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/th.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/th.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tl-ph.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tl-ph.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tlh.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tlh.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tr.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tr.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzl.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzl.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm-latn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm-latn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/tzm.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ug-cn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ug-cn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uk.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uk.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ur.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/ur.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz-latn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz-latn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/uz.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/vi.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/vi.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/x-pseudo.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/x-pseudo.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/yo.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/yo.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-cn.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-hk.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-hk.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-tw.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/dist/vendor/momentjs-locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/examples/acemarkdown.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/examples/acemarkdown.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/acemarkdown.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/acemarkdown.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/alerts.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/alerts.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/all.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/all.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bootstrap.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bootstrap.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bulkfileupload.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/bulkfileupload.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/buttons.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/buttons.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/datetimeselector.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/datetimeselector.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/filewidgets.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/filewidgets.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/focusedpage.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/focusedpage.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/forms.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/forms.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/iframe.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/iframe.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/menu.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/menu.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/mixins.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/mixins.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/modal.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/modal.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/objecttableview.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/objecttableview.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/page-header.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/page-header.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/pager.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/pager.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/roleselect.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/roleselect.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/scaffolding.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/scaffolding.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/submitrow.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/submitrow.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/table.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/table.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/variables.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/variables.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemframe.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemframe.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemvalue.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/itemvalue.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/lists.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listbuilder/lists.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/lists.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/lists.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/target.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/listfilter/target.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/selectableitem.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/selectableitem.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/target.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_base/multiselect2/target.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/menu.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/menu.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/theme.less` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/less/cradmin_theme_default/theme.less`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/detectizr.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/detectizr.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/iosaddtohomescreen.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/iosaddtohomescreen.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/lib.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/lib.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/acemarkdown/acemarkdown.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/acemarkdown/acemarkdown.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/providers.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/backgroundreplace_element/providers.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.spec.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/bulkfileupload.spec.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/fileinfo.tpl.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/fileinfo.tpl.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/rejectedfiles.tpl.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/bulkfileupload/rejectedfiles.tpl.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/calendar/providers.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/calendar/providers.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/collapse/collapse.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/collapse/collapse.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/common/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/common/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/common/providers.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/common/providers.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/clearabletextinput.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/clearabletextinput.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/dateselector.tpl.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/dateselector.tpl.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/datetimewidget.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/datetimewidget.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/filewidget.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/filewidget.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/modelchoicefield.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/modelchoicefield.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/setfieldvalue.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/setfieldvalue.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/usethisbutton.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/forms/usethisbutton.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.spec.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/imagepreview/imagepreview.spec.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/listfilter/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/listfilter/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/services.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/loadmorepager/services.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/menu/menu.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/menu/menu.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/modal/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/modal/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/services.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/multiselect2/services.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/objecttable/objecttable.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/objecttable/objecttable.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/navbar.tpl.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/navbar.tpl.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/pagepreview.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/pagepreview/pagepreview.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/src/lib/scrollfixed/directives.coffee` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/src/lib/scrollfixed/directives.coffee`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.flash.swf` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.flash.swf`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.min.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/FileAPI.min.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.min.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-all.min.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.min.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload-shim.min.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.min.js` & `cradmin_legacy-5.0.0b0/cradmin_legacy/static/cradmin_legacy/thirdparty_js_libs/ng-file-upload-2.1.1/dist/angular-file-upload.min.js`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/superuserui_registry.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/superuserui_registry.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/crapps/djangoapp.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/crapps/djangoapp.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/crapps/djangomodel.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/crapps/djangomodel.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/appdashboardview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/appdashboardview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/dashboardview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/dashboardview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/listview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/listview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/superuserui/views/mixins.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/superuserui/views/mixins.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/base-internal.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/base-internal.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/error.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/error.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/menu.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/menu.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/menuitem.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/menuitem.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/roleselect.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/roleselect.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/standalone-base-internal.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/standalone-base-internal.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/standalone-base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/standalone-base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/acemarkdown/widget.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/acemarkdown/widget.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/collapsed-section-layout.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/collapsed-section-layout.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/submitbutton.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/crispylayouts/submitbutton.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/filewidgets/filewidget.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/filewidgets/filewidget.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/filewidgets/imagewidget.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/filewidgets/imagewidget.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/include/messages.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/include/messages.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused-internal.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused-internal.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/layouts/standalone/focused.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/pagepreview/includes/pagepreview-fullsize-iframe-wrapper.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/create.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/create.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/delete.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/delete.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/formview_base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/formview_base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/loadmorepager-base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/loadmorepager-base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/pager.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/includes/pager.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete-with-archive-image.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete-with-archive-image.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/edit-delete.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/titledescription.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/titledescription.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/use-this.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilder/itemvalue/use-this.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/default.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/default.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-left.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-left.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-right.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-right.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-top.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listbuilderview/filterlist-top.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox/base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox/base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/radio/base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/radio/base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/select/base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/select/base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/textinput/base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/listfilter/django/single/textinput/base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect/formview.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect/formview.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues/itemvalue.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues/itemvalue.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/widget.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget/widget.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer/selected-item.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer/selected-item.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/target_renderer/target.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2/target_renderer/target.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/base.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/base.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/listbuilderfilterview.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/multiselect2view/listbuilderfilterview.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-left.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-left.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-right.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable-filterlist-right.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/viewhelpers/objecttable/objecttable.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/widgets/datetimepicker.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/widgets/datetimepicker.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templates/cradmin_legacy/widgets/modelchoice.django.html` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templates/cradmin_legacy/widgets/modelchoice.django.html`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templatetags/cradmin_legacy_icon_tags.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/cradmin_legacy_icon_tags.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templatetags/cradmin_legacy_image_tags.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/cradmin_legacy_image_tags.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/templatetags/cradmin_legacy_tags.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/templatetags/cradmin_legacy_tags.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/test_abstract_renderable.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_abstract_renderable.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/test_urlutils.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_urlutils.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/formfields/test_email_list.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/formfields/test_email_list.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/sortable/test_sortable.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/sortable/test_sortable.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/sortable/cradmin_sortable_testapp/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/sortable/cradmin_sortable_testapp/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/test_automodelform/test_automodelform.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_automodelform/test_automodelform.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/test_automodelform/cradmin_automodelform_testapp/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/test_automodelform/cradmin_automodelform_testapp/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/utils/test_crhumanize.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/utils/test_crhumanize.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_delete.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_delete.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilderview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilderview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_objecttable.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_objecttable.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/models.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/cradmin_viewhelpers_testapp/models.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_base.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_base.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_itemvalue.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listbuilder/test_itemvalue.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilter.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilter.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilterlist.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_abstractfilterlist.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_filtershandler.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/base/test_filtershandler.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/multi/test_abstractcheckbox.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/multi/test_abstractcheckbox.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractradio.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractradio.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractselect.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/basefilters/single/test_abstractselect.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_select.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_select.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_textinput.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_listfilter/django/single/test_textinput.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_listbuilder_itemvalues.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_listbuilder_itemvalues.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanyview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanyview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanywidget.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_manytomanywidget.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_selected_item_renderer.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_selected_item_renderer.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_target_renderer.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_target_renderer.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_widget_preview_renderer.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/viewhelpers/test_multiselect2/test_widget_preview_renderer.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/tests/views/test_roleselect.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/tests/views/test_roleselect.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/utils/crhumanize.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/utils/crhumanize.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/utils/nulls_last_queryset.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/utils/nulls_last_queryset.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/create.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/create.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/crudbase.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/crudbase.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/delete.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/delete.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/detail.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/detail.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/formbase.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/formbase.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilderview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilderview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/mixins.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/mixins.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2view.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2view.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/objecttable.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/objecttable.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/update.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/update.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/base.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/base.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/itemframe.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/itemframe.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/itemvalue.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/itemvalue.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listbuilder/lists.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listbuilder/lists.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/listfilter_viewmixin.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/listfilter_viewmixin.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/lists.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/lists.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilter.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlist.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlist.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlistchild.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/abstractfilterlistchild.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/base/filtershandler.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/base/filtershandler.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/multi/abstractcheckbox.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/multi/abstractcheckbox.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractradio.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractradio.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractselect.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstractselect.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstracttextinput.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/basefilters/single/abstracttextinput.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/multi/checkbox.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/single/select.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/single/select.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/listfilter/django/single/textinput.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/listfilter/django/single/textinput.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/listbuilder_itemvalues.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/manytomanyview.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/manytomanyview.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/manytomanywidget.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/selected_item_renderer.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/target_renderer.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/target_renderer.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/viewhelpers/multiselect2/widget_preview_renderer.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/viewhelpers/multiselect2/widget_preview_renderer.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/views/roleselect.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/views/roleselect.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/widgets/datetimepicker.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/datetimepicker.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/widgets/filewidgets.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/filewidgets.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/cradmin_legacy/widgets/modelchoice.py` & `cradmin_legacy-5.0.0b0/cradmin_legacy/widgets/modelchoice.py`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/LICENSE` & `cradmin_legacy-5.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/README.md` & `cradmin_legacy-5.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `cradmin_legacy-5.0.0/pyproject.toml` & `cradmin_legacy-5.0.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -80,13 +80,13 @@
     "/cradmin_legacy/static/cradmin_legacy/bower_components",
     "/cradmin_legacy/demo/project/demo/dumps/default.sql",
     "/cradmin_legacy/demo"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "5.0.0"
+version = "5.0.0b0"
 version_files = [
     "cradmin_legacy/__init__.py:__version__"
 ]
 tag_format = "$version"
 update_changelog_on_bump = true
```

### Comparing `cradmin_legacy-5.0.0/PKG-INFO` & `cradmin_legacy-5.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cradmin-legacy
-Version: 5.0.0
+Version: 5.0.0b0
 Summary: Legacy 1.x fork of django cradmin.
 Author: Espen Angell Kristiansen, Tor Johansen, Vegard Angell, Magne Westlie, Stian Julseth
 License: Copyright (c) 2014, Appresso AS 
         All rights reserved. 
         
         Redistribution and use in source and binary forms, with or without 
         modification, are permitted provided that the following conditions are met:
```

