# Comparing `tmp/speech2speech-0.0.1.tar.gz` & `tmp/speech2speech-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech2speech-0.0.1.tar", last modified: Thu Apr 13 06:30:26 2023, max compression
+gzip compressed data, was "speech2speech-0.1.0.tar", last modified: Sat Apr 15 20:17:32 2023, max compression
```

## Comparing `speech2speech-0.0.1.tar` & `speech2speech-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-13 06:30:26.390459 speech2speech-0.0.1/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     4678 2023-04-13 06:30:26.390459 speech2speech-0.0.1/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     4026 2023-04-13 06:11:24.000000 speech2speech-0.0.1/README.md
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      588 2023-04-13 06:29:45.000000 speech2speech-0.0.1/pyproject.toml
--rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-13 06:30:26.390459 speech2speech-0.0.1/setup.cfg
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     8118 2023-04-13 05:47:21.000000 speech2speech-0.0.1/setup.py
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-13 06:30:26.386460 speech2speech-0.0.1/speech2speech/
-drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-13 06:30:26.390459 speech2speech-0.0.1/speech2speech/speech2speech.egg-info/
--rw-rw-r--   0 oem1      (1001) oem1      (1001)     4678 2023-04-13 06:30:26.000000 speech2speech-0.0.1/speech2speech/speech2speech.egg-info/PKG-INFO
--rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-13 06:30:26.000000 speech2speech-0.0.1/speech2speech/speech2speech.egg-info/SOURCES.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-13 06:30:26.000000 speech2speech-0.0.1/speech2speech/speech2speech.egg-info/dependency_links.txt
--rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-13 06:30:26.000000 speech2speech-0.0.1/speech2speech/speech2speech.egg-info/top_level.txt
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-15 20:17:32.374057 speech2speech-0.1.0/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     6155 2023-04-15 20:17:32.374057 speech2speech-0.1.0/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     5438 2023-04-13 12:53:43.000000 speech2speech-0.1.0/README.md
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      612 2023-04-15 20:17:24.000000 speech2speech-0.1.0/pyproject.toml
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)       38 2023-04-15 20:17:32.374057 speech2speech-0.1.0/setup.cfg
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     8181 2023-04-15 20:05:42.000000 speech2speech-0.1.0/setup.py
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-15 20:17:32.370057 speech2speech-0.1.0/speech2speech/
+drwxrwxr-x   0 oem1      (1001) oem1      (1001)        0 2023-04-15 20:17:32.370057 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)     6155 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/PKG-INFO
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)      237 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem1      (1001) oem1      (1001)        1 2023-04-15 20:17:32.000000 speech2speech-0.1.0/speech2speech/speech2speech.egg-info/top_level.txt
```

### Comparing `speech2speech-0.0.1/PKG-INFO` & `speech2speech-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 Metadata-Version: 2.1
 Name: speech2speech
-Version: 0.0.1
-Summary: Speech to machine translation to speech
+Version: 0.1.0
+Summary: Source lang speech to machine translation to target lang speech
 Home-page: https://github.com/rcdalj/speech2speech
 Author: rcdalj
 Author-email: rcdalj1 <rcdalj1@gmail.com>
 Project-URL: Homepage, https://github.com/rcdalj/speech2speech
 Project-URL: Bug Tracker, https://github.com/rcdalj/speech2speech/issues
-Keywords: speech_recognition,machine_translation,text_to_speech,setuptools,development
+Keywords: speech_recognition,machine_translation,text_to_speech,setuptools,development,python-3,chat-gpt,whisper-ai,pyaudio,gtts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # Speech2Speech
 
-Speech2Speech is a Python package that performs vocal recognition of 
-your speech, followed by translation to a target language of your choice, 
-which is then read out loud by a high-quality voice.
+The Speech2Speech Python package **models all phases of speech-to-speech translation**, which include
+- recording speech, 
+- converting speech to text, 
+- translating text to a target language, and 
+- converting the translated text back to speech. 
 
-As long as your speech is in one of the many languages that Chat-GPT can transcribe, you do not have to indicate the source language you are using.
+Each phase of the workflow creates a file, whose name is defined in the config.ini file. Advanced users can start or interrupt the workflow wherever they want by specifying their own files and adapting the config.ini file to refer to them. The user can also launch a specific phase of the workflow by clicking on the corresponding button.
+
+Speech2Speech is designed to be accessible to a **broad audience**, including non-technical users. The package **does not require any specialized software training or user knowledge** and can be used straight out of the box. This makes it incredibly accessible to a wide range of users, including those with visual impairments who can input text by dictating it and have the package read documents aloud.
+
+The package uses PyAudio, Open AI Whisper, Chat-GPT, and Google gttx and can automatically detect the source language used in speech. Users can, therefore, access accurate translations for a **wide range of languages** without having to switch between different translation tools. Although the quality of translation may vary depending on the target language, it is pretty good for popular languages such as English, French, Portuguese, Spanish, German, Dutch and Italian.
 
 Prerequisites
 -----------------------------------------------------------------------------
 Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
 
 1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
-   click on 
-the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
+   click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
 
-2. **Create an OpenAI API Key**: Click on Personal at the right upper corner 
-   and 
-on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
+2. **Create an OpenAI API Key**: Click on Personal at the right upper corner  and on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
 
 3. **Create an Environment Variable to Load Your OpenAI API Key**:
 
-   A. **Ubuntu and Mac**
+   A. **Ubuntu (tested) and Mac (not yet tested)**
    
    Open your terminal. Type the following command to open your shell profile file:
       
          nano ~/.bashrc
       
    Scroll to the bottom of the file and add the following line:
    
          export OPENAI_API_KEY=<YOUR_API_KEY>
       
    Replace <YOUR_API_KEY> with the API key you created in the previous section. Save and close the file by pressing Ctrl + X, then Y, and then Enter. Type the following command to apply the changes:
          
          source ~/.bashrc
          
-   B. **Windows**
+B. **Windows (not yet tested)**
+   
    Right-click on the "Start" button and select "System".
    
    Click on "Advanced system settings".
    
    Click on "Environment Variables".
    
    Under "User variables", click on "New".
@@ -80,19 +84,20 @@
 
 2. Navigate to the directory where your Speech2Speech program is located 
 using the cd command.
 
 3. Type the following command in the terminal to launch Speech2Speech:
 
 
-      streamlit run speech2speech.py
+   `streamlit run speech2speech.py`
+
 
 Workflow
 ----------
-Here's a step-by-step guide on how to use Speech2Speech:
+Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
 1. Click the "Record Audio" button to start recording.
 2. Begin speaking or reading aloud. As long as it supports it, Chat-GPT can 
    automatically detect the 
    language you're speaking, so there's no need to specify it.
 3. Click the "Stop Recording" button to end the recording.
 4. Click the "Transcribe" button to convert your speech into text. The 
@@ -101,12 +106,14 @@
    Language".
 6. Click the "Translate" button to translate the transcription into your 
    chosen target language. The translated text will appear on a blue 
    background after a few seconds.
 7. Click the "Read Translation" button to listen to the translated text.
 8. If you want to repeat the process with a new dictation, click the "Refresh 
    Page" button to reset the page.
+   
+As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
-If Chat-GPT gets stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
+If Chat-GPT or speech2speech get stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
```

### Comparing `speech2speech-0.0.1/README.md` & `speech2speech-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 # Speech2Speech
 
-Speech2Speech is a Python package that performs vocal recognition of 
-your speech, followed by translation to a target language of your choice, 
-which is then read out loud by a high-quality voice.
+The Speech2Speech Python package **models all phases of speech-to-speech translation**, which include
+- recording speech, 
+- converting speech to text, 
+- translating text to a target language, and 
+- converting the translated text back to speech. 
 
-As long as your speech is in one of the many languages that Chat-GPT can transcribe, you do not have to indicate the source language you are using.
+Each phase of the workflow creates a file, whose name is defined in the config.ini file. Advanced users can start or interrupt the workflow wherever they want by specifying their own files and adapting the config.ini file to refer to them. The user can also launch a specific phase of the workflow by clicking on the corresponding button.
+
+Speech2Speech is designed to be accessible to a **broad audience**, including non-technical users. The package **does not require any specialized software training or user knowledge** and can be used straight out of the box. This makes it incredibly accessible to a wide range of users, including those with visual impairments who can input text by dictating it and have the package read documents aloud.
+
+The package uses PyAudio, Open AI Whisper, Chat-GPT, and Google gttx and can automatically detect the source language used in speech. Users can, therefore, access accurate translations for a **wide range of languages** without having to switch between different translation tools. Although the quality of translation may vary depending on the target language, it is pretty good for popular languages such as English, French, Portuguese, Spanish, German, Dutch and Italian.
 
 Prerequisites
 -----------------------------------------------------------------------------
 Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
 
 1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
-   click on 
-the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
+   click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
 
-2. **Create an OpenAI API Key**: Click on Personal at the right upper corner 
-   and 
-on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
+2. **Create an OpenAI API Key**: Click on Personal at the right upper corner  and on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
 
 3. **Create an Environment Variable to Load Your OpenAI API Key**:
 
-   A. **Ubuntu and Mac**
+   A. **Ubuntu (tested) and Mac (not yet tested)**
    
    Open your terminal. Type the following command to open your shell profile file:
       
          nano ~/.bashrc
       
    Scroll to the bottom of the file and add the following line:
    
          export OPENAI_API_KEY=<YOUR_API_KEY>
       
    Replace <YOUR_API_KEY> with the API key you created in the previous section. Save and close the file by pressing Ctrl + X, then Y, and then Enter. Type the following command to apply the changes:
          
          source ~/.bashrc
          
-   B. **Windows**
+B. **Windows (not yet tested)**
+   
    Right-click on the "Start" button and select "System".
    
    Click on "Advanced system settings".
    
    Click on "Environment Variables".
    
    Under "User variables", click on "New".
@@ -64,19 +68,20 @@
 
 2. Navigate to the directory where your Speech2Speech program is located 
 using the cd command.
 
 3. Type the following command in the terminal to launch Speech2Speech:
 
 
-      streamlit run speech2speech.py
+   `streamlit run speech2speech.py`
+
 
 Workflow
 ----------
-Here's a step-by-step guide on how to use Speech2Speech:
+Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
 1. Click the "Record Audio" button to start recording.
 2. Begin speaking or reading aloud. As long as it supports it, Chat-GPT can 
    automatically detect the 
    language you're speaking, so there's no need to specify it.
 3. Click the "Stop Recording" button to end the recording.
 4. Click the "Transcribe" button to convert your speech into text. The 
@@ -85,12 +90,14 @@
    Language".
 6. Click the "Translate" button to translate the transcription into your 
    chosen target language. The translated text will appear on a blue 
    background after a few seconds.
 7. Click the "Read Translation" button to listen to the translated text.
 8. If you want to repeat the process with a new dictation, click the "Refresh 
    Page" button to reset the page.
+   
+As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
-If Chat-GPT gets stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
+If Chat-GPT or speech2speech get stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
```

### Comparing `speech2speech-0.0.1/setup.py` & `speech2speech-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,16 @@
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
     keywords="speech_recognition, machine_translation, text_to_speech, "
-             "setuptools, development",  # Optional
+             "setuptools, development, python-3, chat-gpt, whisper-ai, "
+             "pyaudio, gtts",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
     package_dir={"": "speech2speech"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
```

### Comparing `speech2speech-0.0.1/speech2speech/speech2speech.egg-info/PKG-INFO` & `speech2speech-0.1.0/speech2speech/speech2speech.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 Metadata-Version: 2.1
 Name: speech2speech
-Version: 0.0.1
-Summary: Speech to machine translation to speech
+Version: 0.1.0
+Summary: Source lang speech to machine translation to target lang speech
 Home-page: https://github.com/rcdalj/speech2speech
 Author: rcdalj
 Author-email: rcdalj1 <rcdalj1@gmail.com>
 Project-URL: Homepage, https://github.com/rcdalj/speech2speech
 Project-URL: Bug Tracker, https://github.com/rcdalj/speech2speech/issues
-Keywords: speech_recognition,machine_translation,text_to_speech,setuptools,development
+Keywords: speech_recognition,machine_translation,text_to_speech,setuptools,development,python-3,chat-gpt,whisper-ai,pyaudio,gtts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # Speech2Speech
 
-Speech2Speech is a Python package that performs vocal recognition of 
-your speech, followed by translation to a target language of your choice, 
-which is then read out loud by a high-quality voice.
+The Speech2Speech Python package **models all phases of speech-to-speech translation**, which include
+- recording speech, 
+- converting speech to text, 
+- translating text to a target language, and 
+- converting the translated text back to speech. 
 
-As long as your speech is in one of the many languages that Chat-GPT can transcribe, you do not have to indicate the source language you are using.
+Each phase of the workflow creates a file, whose name is defined in the config.ini file. Advanced users can start or interrupt the workflow wherever they want by specifying their own files and adapting the config.ini file to refer to them. The user can also launch a specific phase of the workflow by clicking on the corresponding button.
+
+Speech2Speech is designed to be accessible to a **broad audience**, including non-technical users. The package **does not require any specialized software training or user knowledge** and can be used straight out of the box. This makes it incredibly accessible to a wide range of users, including those with visual impairments who can input text by dictating it and have the package read documents aloud.
+
+The package uses PyAudio, Open AI Whisper, Chat-GPT, and Google gttx and can automatically detect the source language used in speech. Users can, therefore, access accurate translations for a **wide range of languages** without having to switch between different translation tools. Although the quality of translation may vary depending on the target language, it is pretty good for popular languages such as English, French, Portuguese, Spanish, German, Dutch and Italian.
 
 Prerequisites
 -----------------------------------------------------------------------------
 Before using Speech2Speech, you need to sign up for an OpenAI account, create an API key, and set up an environment variable. Here's how to do it:
 
 1. **Signup and Create an OpenAI Account**: Go to the OpenAI website and 
-   click on 
-the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
+   click on the "Sign up" button in the top right corner. Enter your name, email address, and password in the provided fields, and click on the "Sign up" button. Once you have signed up, you will be directed to the OpenAI dashboard.
 
-2. **Create an OpenAI API Key**: Click on Personal at the right upper corner 
-   and 
-on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
+2. **Create an OpenAI API Key**: Click on Personal at the right upper corner  and on the "View API Keys" tab in the OpenAI dashboard. Click on the "Create new secret key" button. Give your API key a name and select the type of API key you want to create (restricted or full). Once you have created your API key, copy it to your clipboard. Make sure to keep your API key secure, as it provides access to powerful computing resources and data.
 
 3. **Create an Environment Variable to Load Your OpenAI API Key**:
 
-   A. **Ubuntu and Mac**
+   A. **Ubuntu (tested) and Mac (not yet tested)**
    
    Open your terminal. Type the following command to open your shell profile file:
       
          nano ~/.bashrc
       
    Scroll to the bottom of the file and add the following line:
    
          export OPENAI_API_KEY=<YOUR_API_KEY>
       
    Replace <YOUR_API_KEY> with the API key you created in the previous section. Save and close the file by pressing Ctrl + X, then Y, and then Enter. Type the following command to apply the changes:
          
          source ~/.bashrc
          
-   B. **Windows**
+B. **Windows (not yet tested)**
+   
    Right-click on the "Start" button and select "System".
    
    Click on "Advanced system settings".
    
    Click on "Environment Variables".
    
    Under "User variables", click on "New".
@@ -80,19 +84,20 @@
 
 2. Navigate to the directory where your Speech2Speech program is located 
 using the cd command.
 
 3. Type the following command in the terminal to launch Speech2Speech:
 
 
-      streamlit run speech2speech.py
+   `streamlit run speech2speech.py`
+
 
 Workflow
 ----------
-Here's a step-by-step guide on how to use Speech2Speech:
+Here's a step-by-step guide on how to use the full workflow of Speech2Speech:
 
 1. Click the "Record Audio" button to start recording.
 2. Begin speaking or reading aloud. As long as it supports it, Chat-GPT can 
    automatically detect the 
    language you're speaking, so there's no need to specify it.
 3. Click the "Stop Recording" button to end the recording.
 4. Click the "Transcribe" button to convert your speech into text. The 
@@ -101,12 +106,14 @@
    Language".
 6. Click the "Translate" button to translate the transcription into your 
    chosen target language. The translated text will appear on a blue 
    background after a few seconds.
 7. Click the "Read Translation" button to listen to the translated text.
 8. If you want to repeat the process with a new dictation, click the "Refresh 
    Page" button to reset the page.
+   
+As indicated above, you can also use just parts of this full workflow by specifying the name(s) of the file(s) you want to use in the config.ini file and by clicking the relevant button of the user interface.
 
 What to do if you encounter issues
 -------------------------------
 
-If Chat-GPT gets stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
+If Chat-GPT or speech2speech get stuck or you encounter any issues, simply click the "Refresh Page" button to reload the page with the default settings.
```

