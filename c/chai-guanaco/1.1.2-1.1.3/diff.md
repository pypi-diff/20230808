# Comparing `tmp/chai-guanaco-1.1.2.tar.gz` & `tmp/chai-guanaco-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chai-guanaco-1.1.2.tar", last modified: Mon Aug  7 16:17:27 2023, max compression
+gzip compressed data, was "dist/chai-guanaco-1.1.3.tar", last modified: Tue Aug  8 00:20:17 2023, max compression
```

## Comparing `chai-guanaco-1.1.2.tar` & `chai-guanaco-1.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/
--rw-rw-r--   0 alex      (1003) alex      (1003)       72 2023-08-07 16:08:30.000000 chai-guanaco-1.1.2/MANIFEST.in
--rw-rw-r--   0 alex      (1003) alex      (1003)    11603 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/PKG-INFO
--rw-rw-r--   0 alex      (1003) alex      (1003)     9789 2023-08-07 16:08:30.000000 chai-guanaco-1.1.2/README.md
--rw-rw-r--   0 alex      (1003) alex      (1003)       46 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/requirements.txt
--rw-rw-r--   0 alex      (1003) alex      (1003)       38 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/setup.cfg
--rw-rw-r--   0 alex      (1003) alex      (1003)      978 2023-08-07 16:17:24.000000 chai-guanaco-1.1.2/setup.py
-drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/
-drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco/
--rw-rw-r--   0 alex      (1003) alex      (1003)      270 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/__init__.py
--rw-rw-r--   0 alex      (1003) alex      (1003)     4841 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/chat.py
--rw-rw-r--   0 alex      (1003) alex      (1003)     3259 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/feedback.py
--rw-rw-r--   0 alex      (1003) alex      (1003)     1756 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/formatters.py
--rw-rw-r--   0 alex      (1003) alex      (1003)     1966 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/login_cli.py
--rw-rw-r--   0 alex      (1003) alex      (1003)     7397 2023-08-04 23:43:39.000000 chai-guanaco-1.1.2/src/chai_guanaco/metrics.py
-drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/
-drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/
--rw-rw-r--   0 alex      (1003) alex      (1003)     1332 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/blade.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1529 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/captain_wyatt.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     2031 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1305 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/filbert.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1050 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/leo.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1053 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/levi.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1821 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/mr_wilson.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1094 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/nerd_girl.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     2205 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/scaramouche.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     1386 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/story_teller.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     2510 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/vampire_queen.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     2246 2023-08-04 21:30:33.000000 chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/wednesday_addams.json
--rw-rw-r--   0 alex      (1003) alex      (1003)     5474 2023-08-04 21:24:56.000000 chai-guanaco-1.1.2/src/chai_guanaco/submit.py
--rw-rw-r--   0 alex      (1003) alex      (1003)     1945 2023-07-26 22:05:52.000000 chai-guanaco-1.1.2/src/chai_guanaco/utils.py
-drwxrwxr-x   0 alex      (1003) alex      (1003)        0 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/
--rw-rw-r--   0 alex      (1003) alex      (1003)    11603 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1003) alex      (1003)     1199 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1003) alex      (1003)        1 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1003) alex      (1003)       61 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1003) alex      (1003)        1 2023-08-07 15:14:15.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1003) alex      (1003)       46 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1003) alex      (1003)       13 2023-08-07 16:17:27.000000 chai-guanaco-1.1.2/src/chai_guanaco.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10048 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9789 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4841 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3259 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/formatters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/login_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     7397 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/blade.json
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/captain_wyatt.json
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/filbert.json
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/leo.json
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/levi.json
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/mr_wilson.json
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/nerd_girl.json
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/scaramouche.json
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/story_teller.json
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/vampire_queen.json
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2023-08-08 00:20:08.000000 chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/wednesday_addams.json
+-rw-rw-rw-   0 root         (0) root         (0)     5474 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/submit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2023-08-08 00:20:07.000000 chai-guanaco-1.1.3/src/chai_guanaco/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10048 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:20:17.000000 chai-guanaco-1.1.3/src/chai_guanaco.egg-info/top_level.txt
```

### Comparing `chai-guanaco-1.1.2/PKG-INFO` & `chai-guanaco-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,206 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.1.2
+Version: 1.1.3
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
-Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
-        
-        [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
-        [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
-        
-        [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
-        
-        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
-        
-        ## Quick Start
-        
-        [Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
-        
-        
-        ## The Guanaco Guide
-        
-        🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
-        
-        🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
-        
-        🤖 **Model requirements:** Currently, we support *any* models based off [LLaMA 2](https://huggingface.co/docs/transformers/model_doc/llama2) (i.e. 7/13B parameters with LLaMA tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
-        
-        ⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
-        
-        📚 **Rules:** By default, 1 developer key per person, each key can deploy 1 model to users at a time. Message in discord if you would like the limit bumped up 😀
-        
-        
-        ## How Does It Work?
-        
-        -   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
-        -   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
-        -   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
-        -   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
-        -   Cash prizes will be allocated according to your position in the leaderboard 💰
-        
-        [![Chai Pipeline](https://imgur.com/LtMWOAq.png)](https://www.chai-research.com/competition.html)
-        
-        ## 🚀 Getting Started
-        
-        **Getting Developer Key**
-        
-        Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
-        
-        
-        **Installation**
-        
-        Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
-        
-        ```sh
-        pip install chai-guanaco
-        ```
-        
-        For one-off authentication run the following in your terminal:
-        
-        ```sh
-        chai-guanaco login
-        ```
-        
-        And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
-        
-        **Model Submission**
-        
-        Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
-        
-        To submit model simply run:
-        
-        ```python
-        import chai_guanaco as chai
-        
-        model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
-        
-        generation_params = {
-        	'temperature': 1.0,
-        	'repetition_penalty': 1.13,
-        	'top_p': 0.2,
-        	"top_k": 40,
-        	"stopping_words": ['\n'],
-        	"presence_penalty": 0.,
-        	"frequency_penalty": 0.
-        	}
-        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
-        
-        submitter = chai.ModelSubmitter()
-        submission_id = submitter.submit(submission_parameters)
-        ```
-        
-        This will display an animation while your model is being deployed, a typical
-        deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
-        
-        
-        **Chat With Your Model Submission**
-        
-        Once your model is deployed, you can verify its behaviour and raw input by running:
-        
-        ```python
-        chatbot = chai.SubmissionChatbot(submission_id)
-        chatbot.chat('nerd_girl', show_model_input=False)
-        ```
-        
-        Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
-        
-        You can get a list of avaliable bots by running:
-        
-        ```python
-        chatbot.show_avaliable_bots()
-        ```
-        
-        Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
-        
-        ```python
-        chatbot.chat('nerd_girl', show_model_input=True)
-        ```
-        
-        **Getting User Feedback**
-        
-        Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
-        
-        ```python
-        model_feedback = chai.get_feedback(submission_id)
-        model_feedback.sample()
-        ```
-        
-        Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
-        
-        To get all the feedback for your model, run...
-        
-        ```python
-        df = model_feedback.df
-        print(df)
-        ```
-        
-        This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
-        
-        **Getting Live Leaderboard**
-        
-        To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
-        ```python
-        df = chai.display_leaderboard(detailed=False)
-        ```
-        
-        To see how your model performs against other models, run:
-        ```python
-        df = chai.display_leaderboard(detailed=True)
-        ```
-        which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
-        
-        **Re-Submitting Models**
-        
-        Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
-        
-        ```python
-        chai.deactivate_model(submission_id)
-        ```
-        Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
-        
-        **Retrieve Your Model Submission IDs**
-        
-        In case you have forgotten your submission ids / want to view all past submissions, run:
-        
-        ```python
-        submission_ids = chai.get_my_submissions()
-        print(submission_ids)
-        ```
-        Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
-        
-        **Advanced Usage**
-        - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
-        - You can also access the raw feedback data by running
-        	```python
-        	model_feedback = chai.get_feedback(submission_id)
-        	raw_data = model_feedback.raw_data
-        	```
-        - To submit your model with custom formatting, you can create your own
-          `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
-        
-        
-        
-        ## Resources
-        |                                                                        |                                                                                                 |
-        | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
-        | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
-        | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-        | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
-        |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-        |💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
-        | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
-        
-        
-        ## 🦙 Hosted & Sponsored By
-        
-        <a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
-        
-        <a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+[![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
+
+[![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
+[![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
+
+[Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
+
+It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+
+## Quick Start
+
+[Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
+
+
+## The Guanaco Guide
+
+🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
+
+🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
+
+🤖 **Model requirements:** Currently, we support *any* models based off [LLaMA 2](https://huggingface.co/docs/transformers/model_doc/llama2) (i.e. 7/13B parameters with LLaMA tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
+
+⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
+
+📚 **Rules:** By default, 1 developer key per person, each key can deploy 1 model to users at a time. Message in discord if you would like the limit bumped up 😀
+
+
+## How Does It Work?
+
+-   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
+-   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
+-   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
+-   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
+-   Cash prizes will be allocated according to your position in the leaderboard 💰
+
+[![Chai Pipeline](https://imgur.com/LtMWOAq.png)](https://www.chai-research.com/competition.html)
+
+## 🚀 Getting Started
+
+**Getting Developer Key**
+
+Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
+
+
+**Installation**
+
+Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
+
+```sh
+pip install chai-guanaco
+```
+
+For one-off authentication run the following in your terminal:
+
+```sh
+chai-guanaco login
+```
+
+And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+
+**Model Submission**
+
+Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
+
+To submit model simply run:
+
+```python
+import chai_guanaco as chai
+
+model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
+
+generation_params = {
+	'temperature': 1.0,
+	'repetition_penalty': 1.13,
+	'top_p': 0.2,
+	"top_k": 40,
+	"stopping_words": ['\n'],
+	"presence_penalty": 0.,
+	"frequency_penalty": 0.
+	}
+submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
+
+submitter = chai.ModelSubmitter()
+submission_id = submitter.submit(submission_parameters)
+```
+
+This will display an animation while your model is being deployed, a typical
+deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
+
+
+**Chat With Your Model Submission**
+
+Once your model is deployed, you can verify its behaviour and raw input by running:
+
+```python
+chatbot = chai.SubmissionChatbot(submission_id)
+chatbot.chat('nerd_girl', show_model_input=False)
+```
+
+Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+
+You can get a list of avaliable bots by running:
+
+```python
+chatbot.show_avaliable_bots()
+```
+
+Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+
+```python
+chatbot.chat('nerd_girl', show_model_input=True)
+```
+
+**Getting User Feedback**
+
+Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
+
+```python
+model_feedback = chai.get_feedback(submission_id)
+model_feedback.sample()
+```
+
+Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
+
+To get all the feedback for your model, run...
+
+```python
+df = model_feedback.df
+print(df)
+```
+
+This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
+
+**Getting Live Leaderboard**
+
+To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
+```python
+df = chai.display_leaderboard(detailed=False)
+```
+
+To see how your model performs against other models, run:
+```python
+df = chai.display_leaderboard(detailed=True)
+```
+which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
+
+**Re-Submitting Models**
+
+Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
+
+```python
+chai.deactivate_model(submission_id)
+```
+Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
+
+**Retrieve Your Model Submission IDs**
+
+In case you have forgotten your submission ids / want to view all past submissions, run:
+
+```python
+submission_ids = chai.get_my_submissions()
+print(submission_ids)
+```
+Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
+
+**Advanced Usage**
+- This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+- You can also access the raw feedback data by running
+	```python
+	model_feedback = chai.get_feedback(submission_id)
+	raw_data = model_feedback.raw_data
+	```
+- To submit your model with custom formatting, you can create your own
+  `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
+
+
+
+## Resources
+|                                                                        |                                                                                                 |
+| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
+| 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
+| 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
+| 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
+|🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
+|💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
+| ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
+
+
+## 🦙 Hosted & Sponsored By
+
+<a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
+
+<a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
+
+
```

### Comparing `chai-guanaco-1.1.2/README.md` & `chai-guanaco-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/setup.py` & `chai-guanaco-1.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 long_description = (current_dir / "README.md").read_text()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 if os.environ.get('CI_COMMIT_TAG', None):
     version = os.environ['CI_COMMIT_TAG']
+    version = os.environ['CI_COMMIT_TAG'].replace("v", "")
+    version_split = version.split(".")
+    assert len(version_split) == 3, f"Unknown version format {version}, expecting vX.Y.Z"
 else:
     version = "1.1.2"
 
 setup(
     name='chai-guanaco',
     version=version,
     description='Chai Guanaco',
```

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/chat.py` & `chai-guanaco-1.1.3/src/chai_guanaco/chat.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/feedback.py` & `chai-guanaco-1.1.3/src/chai_guanaco/feedback.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/formatters.py` & `chai-guanaco-1.1.3/src/chai_guanaco/formatters.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/login_cli.py` & `chai-guanaco-1.1.3/src/chai_guanaco/login_cli.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/metrics.py` & `chai-guanaco-1.1.3/src/chai_guanaco/metrics.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/blade.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/blade.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/captain_wyatt.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/captain_wyatt.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/coffee_shop_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/filbert.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/filbert.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/leo.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/leo.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/levi.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/levi.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/mr_wilson.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/mr_wilson.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/nerd_girl.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/nerd_girl.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/scaramouche.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/scaramouche.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/story_teller.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/story_teller.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/vampire_queen.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/vampire_queen.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/resources/bot_config/wednesday_addams.json` & `chai-guanaco-1.1.3/src/chai_guanaco/resources/bot_config/wednesday_addams.json`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/submit.py` & `chai-guanaco-1.1.3/src/chai_guanaco/submit.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco/utils.py` & `chai-guanaco-1.1.3/src/chai_guanaco/utils.py`

 * *Files identical despite different names*

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco.egg-info/PKG-INFO` & `chai-guanaco-1.1.3/src/chai_guanaco.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,206 @@
 Metadata-Version: 2.1
 Name: chai-guanaco
-Version: 1.1.2
+Version: 1.1.3
 Summary: Chai Guanaco
 Home-page: https://www.chai-research.com
 Author: Chai Research Corp.
 Author-email: hello@chai-research.com
 License: MIT
-Description: [![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
-        
-        [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
-        [![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
-        
-        [Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
-        
-        It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
-        
-        ## Quick Start
-        
-        [Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
-        
-        
-        ## The Guanaco Guide
-        
-        🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
-        
-        🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
-        
-        🤖 **Model requirements:** Currently, we support *any* models based off [LLaMA 2](https://huggingface.co/docs/transformers/model_doc/llama2) (i.e. 7/13B parameters with LLaMA tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
-        
-        ⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
-        
-        📚 **Rules:** By default, 1 developer key per person, each key can deploy 1 model to users at a time. Message in discord if you would like the limit bumped up 😀
-        
-        
-        ## How Does It Work?
-        
-        -   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
-        -   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
-        -   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
-        -   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
-        -   Cash prizes will be allocated according to your position in the leaderboard 💰
-        
-        [![Chai Pipeline](https://imgur.com/LtMWOAq.png)](https://www.chai-research.com/competition.html)
-        
-        ## 🚀 Getting Started
-        
-        **Getting Developer Key**
-        
-        Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
-        
-        
-        **Installation**
-        
-        Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
-        
-        ```sh
-        pip install chai-guanaco
-        ```
-        
-        For one-off authentication run the following in your terminal:
-        
-        ```sh
-        chai-guanaco login
-        ```
-        
-        And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
-        
-        **Model Submission**
-        
-        Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
-        
-        To submit model simply run:
-        
-        ```python
-        import chai_guanaco as chai
-        
-        model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
-        
-        generation_params = {
-        	'temperature': 1.0,
-        	'repetition_penalty': 1.13,
-        	'top_p': 0.2,
-        	"top_k": 40,
-        	"stopping_words": ['\n'],
-        	"presence_penalty": 0.,
-        	"frequency_penalty": 0.
-        	}
-        submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
-        
-        submitter = chai.ModelSubmitter()
-        submission_id = submitter.submit(submission_parameters)
-        ```
-        
-        This will display an animation while your model is being deployed, a typical
-        deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
-        
-        
-        **Chat With Your Model Submission**
-        
-        Once your model is deployed, you can verify its behaviour and raw input by running:
-        
-        ```python
-        chatbot = chai.SubmissionChatbot(submission_id)
-        chatbot.chat('nerd_girl', show_model_input=False)
-        ```
-        
-        Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
-        
-        You can get a list of avaliable bots by running:
-        
-        ```python
-        chatbot.show_avaliable_bots()
-        ```
-        
-        Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
-        
-        ```python
-        chatbot.chat('nerd_girl', show_model_input=True)
-        ```
-        
-        **Getting User Feedback**
-        
-        Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
-        
-        ```python
-        model_feedback = chai.get_feedback(submission_id)
-        model_feedback.sample()
-        ```
-        
-        Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
-        
-        To get all the feedback for your model, run...
-        
-        ```python
-        df = model_feedback.df
-        print(df)
-        ```
-        
-        This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
-        
-        **Getting Live Leaderboard**
-        
-        To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
-        ```python
-        df = chai.display_leaderboard(detailed=False)
-        ```
-        
-        To see how your model performs against other models, run:
-        ```python
-        df = chai.display_leaderboard(detailed=True)
-        ```
-        which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
-        
-        **Re-Submitting Models**
-        
-        Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
-        
-        ```python
-        chai.deactivate_model(submission_id)
-        ```
-        Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
-        
-        **Retrieve Your Model Submission IDs**
-        
-        In case you have forgotten your submission ids / want to view all past submissions, run:
-        
-        ```python
-        submission_ids = chai.get_my_submissions()
-        print(submission_ids)
-        ```
-        Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
-        
-        **Advanced Usage**
-        - This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
-        - You can also access the raw feedback data by running
-        	```python
-        	model_feedback = chai.get_feedback(submission_id)
-        	raw_data = model_feedback.raw_data
-        	```
-        - To submit your model with custom formatting, you can create your own
-          `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
-        
-        
-        
-        ## Resources
-        |                                                                        |                                                                                                 |
-        | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
-        | 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
-        | 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
-        | 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
-        |🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
-        |💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
-        | ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
-        
-        
-        ## 🦙 Hosted & Sponsored By
-        
-        <a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
-        
-        <a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+[![Guanaco Banner](https://imgur.com/wJHIeAU.png)](https://www.chai-research.com/competition.html)
+
+[![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
+[![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)
+
+[Chai Guanaco](https://www.chai-research.com/competition.html) is part of the Chai Guanaco Competition, accelerating community AGI.
+
+It's the world's first open community challenge with real-user evaluations. You can submit any GPT-J based 6B models, it will be directly deployed on the [Chai App](http://tosto.re/chaiapp) where our over 500K daily active users will be providing live feedback. Get to top of the leaderboard and share the $1 million cash prize!
+
+## Quick Start
+
+[Chai Guanaco Jupyter Notebook Quickstart](https://datalore.jetbrains.com/notebook/ABxxIKqVGejPnF8zH6zFpx/WQd6vDlfCDux5wzuoAeF8m)
+
+
+## The Guanaco Guide
+
+🥇 **Evaluation & Prizes:** Depending on the phase of the competition, a suite of user-level evaluation metrics will be used (i.e. thumbs up / thumbs down rate). Your model will be ranked in real-time compared with other models, you can view the leaderboard at anytime with the pip package
+
+🕵️ **Real-time user feedback:** After your model is deployed, it will go through an safety + integrity checker, once passed, it will be deployed directly to our users who will provide written feedback that you can view via the pip package.
+
+🤖 **Model requirements:** Currently, we support *any* models based off [LLaMA 2](https://huggingface.co/docs/transformers/model_doc/llama2) (i.e. 7/13B parameters with LLaMA tokenizer). All you need to do is push your model directly to huggingface. Support for more model types is coming soon!
+
+⚙️ **Sampling parameters:** During submission, we allow for custom model generation parameters such as temperature. Once your model is deployed on our platform, it will be using the parameters you've provided to generate chat completions.
+
+📚 **Rules:** By default, 1 developer key per person, each key can deploy 1 model to users at a time. Message in discord if you would like the limit bumped up 😀
+
+
+## How Does It Work?
+
+-   The `chai_guanaco` pip package provides a way to easily submit your language model, all you need to do is ensure it is on HuggingFace 🤗
+-   We will automatically **Tritonize** your model for fast inference and host it in our internal GPU cluster 🚀
+-   Once deployed, Chai users on our platform who enter the **arena mode** will be rating your model directly, providing you with both quantatitive and verbal feedback 📈
+-   Both the public leaderboard and **user feedback** for your model can be directly downloaded via the `chai_guanaco` package 🧠
+-   Cash prizes will be allocated according to your position in the leaderboard 💰
+
+[![Chai Pipeline](https://imgur.com/LtMWOAq.png)](https://www.chai-research.com/competition.html)
+
+## 🚀 Getting Started
+
+**Getting Developer Key**
+
+Join the [competition discord](https://discord.gg/7mXdjAkw2s), introduce yourself and ask for a developer key. Login-based authentication is coming next 🤗
+
+
+**Installation**
+
+Use [pip](https://github.com/pypa/pip) to install the Chai Guanaco package
+
+```sh
+pip install chai-guanaco
+```
+
+For one-off authentication run the following in your terminal:
+
+```sh
+chai-guanaco login
+```
+
+And pass in your developer key when prompted, you can always logout using `chai-guanaco logout`.
+
+**Model Submission**
+
+Upload any Llama based language model *with a tokenizer* to huggingface, i.e. [NousResearch/Llama-2-7b-chat-hf](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf). Read [this guide](https://huggingface.co/docs/transformers/model_sharing) if you are unsure. Click the *Use in Transformers* button in huggingface to get the your huggingface model ID (i.e. "NousResearch/Llama-2-7b-chat-hf")
+
+To submit model simply run:
+
+```python
+import chai_guanaco as chai
+
+model_url = "NousResearch/Llama-2-7b-chat-hf" # Your model URL
+
+generation_params = {
+	'temperature': 1.0,
+	'repetition_penalty': 1.13,
+	'top_p': 0.2,
+	"top_k": 40,
+	"stopping_words": ['\n'],
+	"presence_penalty": 0.,
+	"frequency_penalty": 0.
+	}
+submission_parameters = {'model_repo': model_url, 'generation_params': generation_params, 'model_name': 'my-awesome-llama'}
+
+submitter = chai.ModelSubmitter()
+submission_id = submitter.submit(submission_parameters)
+```
+
+This will display an animation while your model is being deployed, a typical
+deployment takes approximately 10 minutes. Note the `model_name` parameter is used for show-casing your model on the leaderboard and it should help you with identifying your model
+
+
+**Chat With Your Model Submission**
+
+Once your model is deployed, you can verify its behaviour and raw input by running:
+
+```python
+chatbot = chai.SubmissionChatbot(submission_id)
+chatbot.chat('nerd_girl', show_model_input=False)
+```
+
+Here you can have a dialog with one of the bots we have provided. To quit the chat, simply enter "exit". Note that, in order to prevent spamming, each model submission is limited to 1000 chat messages from the Chai Guanaco pip package.
+
+You can get a list of avaliable bots by running:
+
+```python
+chatbot.show_avaliable_bots()
+```
+
+Finally, to enter a chat session that prints out the raw input that was fed into your model at each turn of the conversation, you can run:
+
+```python
+chatbot.chat('nerd_girl', show_model_input=True)
+```
+
+**Getting User Feedback**
+
+Once your model has been submitted, it is automatically deployed to the Chai Platform where real-life users will evaluate your model performance. To view their feedback, run:
+
+```python
+model_feedback = chai.get_feedback(submission_id)
+model_feedback.sample()
+```
+
+Which will print out one of the users' conversation, together with meta information associated with the conversation (i.e. rating and user feedback).
+
+To get all the feedback for your model, run...
+
+```python
+df = model_feedback.df
+print(df)
+```
+
+This outputs a Pandas `DataFrame`, where each row corresponds to a user conversation with your model, together with their feedback.
+
+**Getting Live Leaderboard**
+
+To view the public leaderboard used to determine prizes (which only shows the best model submitted by each developer):
+```python
+df = chai.display_leaderboard(detailed=False)
+```
+
+To see how your model performs against other models, run:
+```python
+df = chai.display_leaderboard(detailed=True)
+```
+which prints out the current leaderboard according to the most recent competition metrics, you can also access raw leaderboard is dumped to `df`
+
+**Re-Submitting Models**
+
+Because it is a competition, you are allowed to test a single model at any given time. However, you can deactivate a model and submit a new one. To do this, simply run:
+
+```python
+chai.deactivate_model(submission_id)
+```
+Which will deactive your model, don't worry, all the model feedback will still be saved, it just means the model will no longer be exposed to users. You can then re-submit by repeating the model submission step.
+
+**Retrieve Your Model Submission IDs**
+
+In case you have forgotten your submission ids / want to view all past submissions, run:
+
+```python
+submission_ids = chai.get_my_submissions()
+print(submission_ids)
+```
+Here you will see all your model submission_ids along with their status, which is either `failed`, `inactive` or `deployed`.
+
+**Advanced Usage**
+- This package caches various data, such as your developer key, in the folder `~/.chai-guanaco`. To change this, you can set the environment variable `GUANACO_DATA_DIR` to point to a different folder. You may need to re-run `chai-guanaco login` to update the cached developer key.
+- You can also access the raw feedback data by running
+	```python
+	model_feedback = chai.get_feedback(submission_id)
+	raw_data = model_feedback.raw_data
+	```
+- To submit your model with custom formatting, you can create your own
+  `PromptFormatter`. For more details and examples, please see [here](https://wild-chatter-b52.notion.site/Guanaco-Custom-Formatters-1f64f94b9cf54c819a341988aec5766a).
+
+
+
+## Resources
+|                                                                        |                                                                                                 |
+| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------|
+| 📒 [Fine tuning guide](https://huggingface.co/docs/transformers/training) | Guide on language model finetuning                                                           |
+| 💾 [Datasets](https://dataset-ideas.tiiny.site/) | Curated list of open-sourced datasets to get started with finetuning                                                  |
+| 💖 [Guanaco Discord](https://discord.gg/7mXdjAkw2s)                   | Our Guanaco competition discord                                                          |
+|🚀 [Deepspeed Guide](https://huggingface.co/docs/transformers/main_classes/deepspeed)     | Guide for training with Deepspeed (faster training without GPU bottleneck)    |
+|💬 [Example Conversations](https://huggingface.co/datasets/ChaiML/100_example_conversations)     | Here you can find 100 example conversations from the Chai Platform     |
+| ⚒️ [Build with us](https://boards.greenhouse.io/nexus/jobs/5319721003)| If you think what we are building is cool, join us!|
+
+
+## 🦙 Hosted & Sponsored By
+
+<a href="https://www.chai-research.com/"><img src="https://imgur.com/u3rOQDJ.png" alt="Chai Logo" height="90"/></a>
+
+<a href="https://www.coreweave.com/"><img src="https://imgur.com/oJyuH8q.png" alt="Coreweave Logo" height="70"/></a>
+
+
```

### Comparing `chai-guanaco-1.1.2/src/chai_guanaco.egg-info/SOURCES.txt` & `chai-guanaco-1.1.3/src/chai_guanaco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

