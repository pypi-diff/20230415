# Comparing `tmp/TBForms-0.9.8.tar.gz` & `tmp/TBForms-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TBForms-0.9.8.tar", last modified: Thu Jan 27 19:50:42 2022, max compression
+gzip compressed data, was "/Users/vlad/Desktop/war/TBForms/dist/tmpb2xn1fc6/TBForms-0.9.9.tar", last modified: Wed Mar 16 23:14:42 2022, max compression
```

## Comparing `TBForms-0.9.8.tar` & `TBForms-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 vladka    (1000) vladka    (1000)        0 2022-01-27 19:50:42.000000 TBForms-0.9.8/
--rw-rw-r--   0 vladka    (1000) vladka    (1000)      736 2022-01-27 19:50:17.000000 TBForms-0.9.8/setup.py
--rw-rw-r--   0 vladka    (1000) vladka    (1000)     1065 2021-09-20 12:49:56.000000 TBForms-0.9.8/LICENSE
--rw-r--r--   0 vladka    (1000) vladka    (1000)    14692 2022-01-27 19:50:42.000000 TBForms-0.9.8/PKG-INFO
-drwxr-xr-x   0 vladka    (1000) vladka    (1000)        0 2022-01-27 19:50:42.000000 TBForms-0.9.8/TBForms.egg-info/
--rw-rw-r--   0 vladka    (1000) vladka    (1000)      284 2022-01-27 19:50:42.000000 TBForms-0.9.8/TBForms.egg-info/SOURCES.txt
--rw-rw-r--   0 vladka    (1000) vladka    (1000)    14692 2022-01-27 19:50:42.000000 TBForms-0.9.8/TBForms.egg-info/PKG-INFO
--rw-rw-r--   0 vladka    (1000) vladka    (1000)       22 2022-01-27 19:50:42.000000 TBForms-0.9.8/TBForms.egg-info/requires.txt
--rw-rw-r--   0 vladka    (1000) vladka    (1000)        1 2022-01-27 19:50:42.000000 TBForms-0.9.8/TBForms.egg-info/dependency_links.txt
--rw-rw-r--   0 vladka    (1000) vladka    (1000)        9 2022-01-27 19:50:42.000000 TBForms-0.9.8/TBForms.egg-info/top_level.txt
--rw-rw-r--   0 vladka    (1000) vladka    (1000)    14165 2021-09-29 18:41:45.000000 TBForms-0.9.8/README.md
--rw-r--r--   0 vladka    (1000) vladka    (1000)       38 2022-01-27 19:50:42.000000 TBForms-0.9.8/setup.cfg
-drwxr-xr-x   0 vladka    (1000) vladka    (1000)        0 2022-01-27 19:50:42.000000 TBForms-0.9.8/tb_forms/
--rw-rw-r--   0 vladka    (1000) vladka    (1000)    23566 2022-01-27 19:50:21.000000 TBForms-0.9.8/tb_forms/__init__.py
--rw-rw-r--   0 vladka    (1000) vladka    (1000)      876 2021-10-01 18:15:17.000000 TBForms-0.9.8/tb_forms/tbf_types.py
--rw-rw-r--   0 vladka    (1000) vladka    (1000)    14895 2021-10-01 18:15:53.000000 TBForms-0.9.8/tb_forms/fields.py
--rw-rw-r--   0 vladka    (1000) vladka    (1000)     5442 2021-09-04 14:50:56.000000 TBForms-0.9.8/tb_forms/validators.py
--rw-rw-r--   0 vladka    (1000) vladka    (1000)     3803 2021-09-20 20:14:54.000000 TBForms-0.9.8/tb_forms/tb_fsm.py
+drwxr-xr-x   0 vlad       (501) staff       (20)        0 2022-03-16 23:14:42.000000 TBForms-0.9.9/
+-rw-r--r--   0 vlad       (501) staff       (20)     1065 2022-03-16 16:42:56.000000 TBForms-0.9.9/LICENSE
+-rw-r--r--   0 vlad       (501) staff       (20)    14692 2022-03-16 23:14:42.000000 TBForms-0.9.9/PKG-INFO
+-rw-r--r--   0 vlad       (501) staff       (20)    14165 2022-03-16 16:42:56.000000 TBForms-0.9.9/README.md
+drwxr-xr-x   0 vlad       (501) staff       (20)        0 2022-03-16 23:14:42.000000 TBForms-0.9.9/TBForms.egg-info/
+-rw-r--r--   0 vlad       (501) staff       (20)    14692 2022-03-16 23:14:42.000000 TBForms-0.9.9/TBForms.egg-info/PKG-INFO
+-rw-r--r--   0 vlad       (501) staff       (20)      284 2022-03-16 23:14:42.000000 TBForms-0.9.9/TBForms.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad       (501) staff       (20)        1 2022-03-16 23:14:42.000000 TBForms-0.9.9/TBForms.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad       (501) staff       (20)       22 2022-03-16 23:14:42.000000 TBForms-0.9.9/TBForms.egg-info/requires.txt
+-rw-r--r--   0 vlad       (501) staff       (20)        9 2022-03-16 23:14:42.000000 TBForms-0.9.9/TBForms.egg-info/top_level.txt
+-rw-r--r--   0 vlad       (501) staff       (20)       38 2022-03-16 23:14:42.000000 TBForms-0.9.9/setup.cfg
+-rw-r--r--   0 vlad       (501) staff       (20)      736 2022-03-16 23:13:05.000000 TBForms-0.9.9/setup.py
+drwxr-xr-x   0 vlad       (501) staff       (20)        0 2022-03-16 23:14:42.000000 TBForms-0.9.9/tb_forms/
+-rw-r--r--   0 vlad       (501) staff       (20)    23915 2022-03-16 23:12:30.000000 TBForms-0.9.9/tb_forms/__init__.py
+-rw-r--r--   0 vlad       (501) staff       (20)    18920 2022-03-16 23:10:40.000000 TBForms-0.9.9/tb_forms/fields.py
+-rw-r--r--   0 vlad       (501) staff       (20)     3803 2022-03-16 16:42:58.000000 TBForms-0.9.9/tb_forms/tb_fsm.py
+-rw-r--r--   0 vlad       (501) staff       (20)      876 2022-03-16 16:42:58.000000 TBForms-0.9.9/tb_forms/tbf_types.py
+-rw-r--r--   0 vlad       (501) staff       (20)     5442 2022-03-16 16:42:58.000000 TBForms-0.9.9/tb_forms/validators.py
```

### Comparing `TBForms-0.9.8/setup.py` & `TBForms-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "pyTelegramBotAPI",
     "dill"
 
 ]
 
 setuptools.setup(
 	name="TBForms",
-	version="0.9.8",
+	version="0.9.9",
 	author="watdev",
 	author_email="v.liubachevskyi@gmail.com",
 	description="Small extension for pyTelegramBotAPI library for building interactive forms in Telegram bots.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/wathipol/TBForms",
 	packages=setuptools.find_packages(),
```

### Comparing `TBForms-0.9.8/LICENSE` & `TBForms-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TBForms-0.9.8/PKG-INFO` & `TBForms-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TBForms
-Version: 0.9.8
+Version: 0.9.9
 Summary: Small extension for pyTelegramBotAPI library for building interactive forms in Telegram bots.
 Home-page: https://github.com/wathipol/TBForms
 Author: watdev
 Author-email: v.liubachevskyi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `TBForms-0.9.8/TBForms.egg-info/PKG-INFO` & `TBForms-0.9.9/TBForms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TBForms
-Version: 0.9.8
+Version: 0.9.9
 Summary: Small extension for pyTelegramBotAPI library for building interactive forms in Telegram bots.
 Home-page: https://github.com/wathipol/TBForms
 Author: watdev
 Author-email: v.liubachevskyi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `TBForms-0.9.8/README.md` & `TBForms-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `TBForms-0.9.8/tb_forms/__init__.py` & `TBForms-0.9.9/tb_forms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from . import validators
 from .tbf_types import FormEvent
 from .tb_fsm import TB_FORM_TAG,DEFAULT_CANCEl_CALLBACK,FIELD_CLICK_CALLBACK_DATA_PATTERN,FSM_FORM_IDE,DEFAULT_SUBMIT_CALLBACK,FSM_GET_FIELD_VALUE,DEFAULT_CANCEl_FORM_CALLBACK,DEFAULT_VALUE_FROM_CALLBACK_PATTERN
 from collections import namedtuple
 import pickle
 import types as build_in_types
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 class EventCollector:
     _submit_collector = {}
     _cancel_collector = {}
     _global_cancel = None
     _global_submit = None
 
@@ -75,16 +75,17 @@
                     return False
             else:
                 if fsm_data.state != FSM_GET_FIELD_VALUE:
                     return False
 
             form = BaseForm.form_loads(fsm_data.args.form)
             settings = self._get_form_settings(form,prepare_update=user_id)
-            if fsm_data.args.from_callback and settings["FREEZE_MODE"]:
-                return True
+            if hasattr(fsm_data.args, 'from_callback'):
+                if fsm_data.args.from_callback and settings["FREEZE_MODE"]:
+                    return True
             return False
 
 
         # Запрет на сообщения до закрытия формы (Запрос значений)
         @bot.message_handler(func=lambda message: True and __check_already_input_only_from_callback_mode(message.chat.id))
         def cath_stop_freeze_events_on_from_callback_getting(message):
             self.stop_freeze_event(message)
@@ -307,14 +308,15 @@
         if field.value_from_callback:
             keyboard = field.create_variables_keys()
         else:
             keyboard = types.InlineKeyboardMarkup()
         cancel_key = types.InlineKeyboardButton(text=settings["CANCEL_BUTTON_TEXT"], callback_data=settings["CANCEL_CALLBACK"])
         if not field.without_system_key:
             keyboard.add(cancel_key)
+        field.before_input_update(self,form,call)
         self.bot.delete_message(call.message.chat.id,call.message.message_id)
         msg = self.bot.send_message(call.from_user.id,text,reply_markup=keyboard)
         form.last_msg_id = msg.message_id
         self.fsm.set_state(call.from_user.id,FSM_GET_FIELD_VALUE,form=form._form_dumps(),field_id=field._id,from_callback=field.value_from_callback)
 
     def submit_form(self,call):
         form_status = self.fsm.check_already_form(int(call.from_user.id))
@@ -366,14 +368,19 @@
 
     def msg_mode_input(self,message):
         state_data = self.fsm.get_state(int(message.from_user.id))
         form = BaseForm.form_loads(state_data.args.form)
         settings = self._get_form_settings(form,prepare_update=message.chat.id)
         f_id = state_data.args.field_id
         field = form.get_field_by_id(f_id)
+
+        if field.value_from_message_manual_mode:
+            field.manualy_handle_message(self,message,form)
+            return
+        field.after_input_update(self,form,message)
         new_value = message.text
         valid = True
         if not field.validate(message):
             valid = False
         else:
             field.value = field.format_return_value(message)
         event = FormEvent("field_input",sub_event_type="msg",event_data=field)
@@ -385,22 +392,24 @@
             error_text = settings["INVALID_INPUT_TEXT"]
             if field.error_message:
                 error_text = field.error_message
             elif form.form_global_error_message:
                 error_text = form.form_global_error_message
             self.bot.reply_to(message,error_text)
 
+    
     def callback_mode_input(self,call):
         state_data = self.fsm.get_state(int(call.from_user.id))
         form = BaseForm.form_loads(state_data.args.form)
         f_id = state_data.args.field_id
         field = form.get_field_by_id(f_id)
         if field.value_from_callback_manual_mode:
             field.manualy_handle_callback(self,call,form)
             return
+        field.after_input_update(self,form,call)
         new_value_id = call.data.split(":")[2]
         new_value = field.get_variable_data(new_value_id)
         field.value = field.format_return_value(new_value)
         self.bot.delete_message(call.message.chat.id,call.message.message_id)
         event = FormEvent("field_input",sub_event_type="callback",event_data=field)
         form.event_listener(event,form.create_update_form_object(action="event_callback"))
         msg = self.send_form(call.from_user.id,form,need_init=False)
```

### Comparing `TBForms-0.9.8/tb_forms/tbf_types.py` & `TBForms-0.9.9/tb_forms/tbf_types.py`

 * *Files identical despite different names*

### Comparing `TBForms-0.9.8/tb_forms/fields.py` & `TBForms-0.9.9/tb_forms/fields.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import random
 import string
 import dill
 from . import validators as fvalidators
 from .validators import all_content_types,Validator
 from .tbf_types import FormEvent
 from telebot import types
-from .tb_fsm import TB_FORM_TAG,DEFAULT_CANCEl_CALLBACK,FIELD_CLICK_CALLBACK_DATA_PATTERN,DEFAULT_VALUE_FROM_CALLBACK_PATTERN,FSM_GET_FIELD_VALUE
+from .tb_fsm import (
+    TB_FORM_TAG,DEFAULT_CANCEl_CALLBACK,
+    FIELD_CLICK_CALLBACK_DATA_PATTERN,
+    DEFAULT_VALUE_FROM_CALLBACK_PATTERN,
+    FSM_GET_FIELD_VALUE,
+    FSM_FORM_IDE
+)
+
 
 def split_list(arr, wanted_parts=1):
     """Разбить список на подсписки"""
     arrs = []
     while len(arr) > wanted_parts:
         pice = arr[:wanted_parts]
         arrs.append(pice)
         arr = arr[wanted_parts:]
     arrs.append(arr)
     return arrs
 
 
 
 def islambda(v):
-  LAMBDA = lambda:0
-  return isinstance(v, type(LAMBDA)) and v.__name__ == LAMBDA.__name__
+    LAMBDA = lambda:0
+    return isinstance(v, type(LAMBDA)) and v.__name__ == LAMBDA.__name__
 
 
 class DillPickle:
     """ Обёртка для сериализации лямбда функций и других типов без поддержки """
     def __init__(self, e):
         self.e = e
 
@@ -61,14 +68,15 @@
         self.input_text = input_text
         self.validators = validators
         self.required = required
         self.read_only = read_only
         self._id = Field._generate_id(self._id_len)
         self.value_from_callback = value_from_callback
         self.value_from_callback_manual_mode = False
+        self.value_from_message_manual_mode = False
         self.without_system_key = False
         self.value = default_value
         self.variable_data = {}
         self.error_message = error_message
         self.validators = self._fix_validators_type(self.validators)
         self.field_hidden_data = field_hidden_data
 
@@ -94,14 +102,20 @@
             else:
                 if not hasattr(validator, '__call__'):
                     continue
                 if not validator(upd):
                     return False
         return True
 
+    def before_input_update(self,tbf,form,update):
+        pass
+
+    def after_input_update(self,tbf,form,update):
+        pass
+
     def field_validator(self,upd):
         return True
 
     def _append_variable_data(self,data) -> str:
         v_id = Field._generate_id(self._id_len)
         self.variable_data[v_id] = data
         return v_id
@@ -109,14 +123,17 @@
     def get_variable_data(self,v_id: str):
         if v_id in list(self.variable_data.keys()):
             return self.variable_data[v_id]
 
     def manualy_handle_callback(self,tbf,call,form):
         pass
 
+    def manualy_handle_message(self,tbf,message,form):
+        pass
+
 
     def create_variables_keys(self):
         """При использовании режима value_from_callback,
             Этот метод нужно переопределить для создания клавиатуры выбора
         """
         pass
 
@@ -344,7 +361,80 @@
 
     def message_text_data_format(self):
         if self.value == None:
             return ""
         if self.multiple:
             return ",".join(self.value)
         return str(self.value)
+
+
+
+
+class ListField(Field):
+    def __init__(self,title=None,input_text=None,save_button_text="Save({}) 💾",validators=[],required=True,read_only=False,error_message=None,min_len=1,max_len=None,default_value=None,field_hidden_data=None):
+        all_validators = []
+        for validator in validators:
+            all_validators.append(validator)
+        super().__init__(title=title,input_text=input_text,validators=all_validators,required=required,read_only=read_only,error_message=error_message,default_value=default_value,field_hidden_data=field_hidden_data)
+        self.save_button_text = save_button_text        
+        self.value_from_message_manual_mode = True
+        self.value_from_callback_manual_mode = True
+        self.min_len = min_len
+        self.max_len = max_len
+
+
+    def format_return_value(self,upd):
+        return upd.text
+
+    def before_input_update(self,tbf,form,update):
+        self.value = None
+
+
+    def manualy_handle_callback(self,tbf,call,form):
+        new_value_id = call.data.split(":")[2]
+        settings = tbf._get_form_settings(form,prepare_update=call.from_user.id)
+        
+        if str(new_value_id) == "save_field":
+            event = FormEvent("field_input",sub_event_type="msg",event_data=self)
+            form.event_listener(event,form.create_update_form_object(action="event_callback"))
+            return tbf.send_form(call.message.chat.id,form,need_init=False)
+        
+        elif str(new_value_id) == "cancel_field":
+            self.value = None
+            idle_state = "{}:{}".format(FSM_FORM_IDE,form._form_id)
+            tbf.fsm.set_state(int(call.from_user.id),idle_state,form=form._form_dumps())
+            tbf.bot.delete_message(call.message.chat.id,call.message.message_id)
+            return tbf.send_form(call.from_user.id,form,need_init=False)
+
+    def manualy_handle_message(self,tbf,message,form):
+        new_value = message.text
+        settings = tbf._get_form_settings(form,prepare_update=message.chat.id)
+        valid = True
+        if not self.validate(message):
+            valid = False
+        else:
+            if not self.value or not isinstance(self.value,list):
+                self.value = []
+            self.value.append(self.format_return_value(message))
+            if not (self.max_len and len(self.value) == self.max_len):
+                new_keyboard =  keyboard = types.InlineKeyboardMarkup()
+                if len(self.value) >= self.min_len:
+                    new_keyboard.row(types.InlineKeyboardButton(text=str(self.save_button_text).format(len(self.value)), callback_data=DEFAULT_VALUE_FROM_CALLBACK_PATTERN.format("save_field"))) 
+                else:
+                    new_keyboard.row(types.InlineKeyboardButton(text=settings["CANCEL_BUTTON_TEXT"], callback_data=DEFAULT_VALUE_FROM_CALLBACK_PATTERN.format("cancel_field"))) 
+                tbf.fsm.set_state(message.from_user.id,FSM_GET_FIELD_VALUE, form=form._form_dumps(),field_id=self._id)
+                msg = tbf.bot.send_message(message.chat.id,self.input_text,reply_markup=new_keyboard)
+                return msg
+        event = FormEvent("field_input",sub_event_type="msg",event_data=self)
+        if not valid:
+            event.event_type = "field_input_invalid"
+        form.event_listener(event,form.create_update_form_object(action="event_callback"))
+        msg = tbf.send_form(message.from_user.id,form,need_init=False)
+        if not valid:
+            error_text = settings["INVALID_INPUT_TEXT"]
+            if field.error_message:
+                error_text = field.error_message
+            elif form.form_global_error_message:
+                error_text = form.form_global_error_message
+            self.bot.reply_to(message,error_text)
+
+
```

### Comparing `TBForms-0.9.8/tb_forms/validators.py` & `TBForms-0.9.9/tb_forms/validators.py`

 * *Files identical despite different names*

### Comparing `TBForms-0.9.8/tb_forms/tb_fsm.py` & `TBForms-0.9.9/tb_forms/tb_fsm.py`

 * *Files identical despite different names*

