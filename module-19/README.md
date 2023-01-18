<img src="../images/extra/banner_aws.png" alt="aws" width=80 height=50 /> [General Content AWS Cloud][1]


[1]: https://github.com/weder96/aws-certification-learning

# Módulo 19: Machine Learning

## Content
1.  <a href="#section-01"> Amazon Comprehend </a>
2.  <a href="#section-02"> Amazon Forecast </a>
3.  <a href="#section-03"> Amazon Fraud Detector </a>
4.  <a href="#section-04"> Amazon Kendra </a>
5.  <a href="#section-05"> Amazon Lex </a>
6.  <a href="#section-06"> Amazon Polly </a>
7.  <a href="#section-07"> Amazon Rekognition </a>
8.  <a href="#section-08"> Amazon SageMaker </a>
9.  <a href="#section-09"> Amazon Textract </a>
10. <a href="#section-10"> Amazon Transcribe </a>
11. <a href="#section-11"> Amazon Translate </a>

![Amazon Comprehend](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Comprehend_64.svg "Amazon Comprehend")
![Amazon Forecast](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Forecast_64.svg "Amazon Forecast")
![Amazon Fraud Detector](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Fraud-Detector_64.svg "Amazon Fraud Detector")
![Amazon Kendra](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Kendra_64.svg "Amazon Kendra")
![Amazon Lex](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Lex_64.svg "Amazon Lex")
![Amazon Polly](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Polly_64.svg "Polly")
![Amazon Rekognition](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Rekognition_64.svg "Amazon Rekognition")
![Amazon SageMaker](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-SageMaker_64.svg "Amazon SageMaker")
![Amazon Textract](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Textract_64.svg "Amazon Textract")
![Amazon Transcribe](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Transcribe_64.svg "Amazon Transcribe")
![Amazon Translate](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Translate_64.svg "Amazon Translate")


***************************************************************************************************
## <a id="section-01"> </a> **1 - Amazon Comprehend**

![Amazon Comprehend](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Comprehend_64.svg "Amazon Comprehend")

**Definitions**

### **What is Amazon Comprehend?**
- A managed Natural Language Processing (NLP) service that you can use to extract meaningful information from unstructured texts so you can analyze them in a human-like context.
- It is an off-the-shelf solution that does not require deep machine learning expertise to get started.
- Works with social media feeds, web pages, comments, product reviews, articles, or emails.
- Can analyze texts in real-time by using built-in and custom models.
- Also offers medical insights and protected health information (PHI) detection via **Amazon Comprehend Medical**

### **Amazon Comprehend Common Use Cases**
- Sentiment analysis for social media posts
- Organize documents by topics
- Knowledge management and discovery
- Classifies support tickets for better issue handling
- Medical cohort analysis
- Identify personally identifiable information (PII) in documents.
- Identify protected health information (PHI) in documents


### **Amazon Comprehend generates insights in six (6) categories:**
- **Entities**
    - Detects and categorizes real-world objects like date, organization, person, quantity, brands, or even a title given to a song or movie.
    - **Custom Entity Recognition**
        - Allows you to identify new entities that are not supported by the preset entities. 
        - This is useful if you want to extract entities that are specific only to your business, such as product codes.
- **Sentiment**
    - Detects and classifies emotions into neutral, positive, negative, or mixed.
- **Language**
    - Detects the language used in a text by using identifiers from RFC 5646. 
    - Useful for multilingual companies or applications.
- **Key Phrases**
    - A key phrase refers to a noun or a noun phrase that describes a particular thing.
- **Personally Identifiable Information (PII)**
    - Determines sensitive information that could be used to identify a person, such as full name, birth date, bank account number, phone number, or email.
- **Syntax**
    - Determine the different parts of speech used in the document, such as noun, pronoun, verb, adjective, adverb, etc.


### **Amazon Comprehend Pricing**
- Charges are based on units where a single unit is equal to 100 characters. 
- 3 unit (300 characters) minimum charge per request.
- All insights except for Syntax analysis are charged for $0.0001 per 10M units. Syntax Analysis is charged for $0.00005 per 10M units.
- Topic Modeling has a flat rate of $1.00 per job.

**Cheat Sheets**

https://tutorialsdojo.com/amazon-comprehend/

**References:**

https://aws.amazon.com/comprehend/

https://docs.aws.amazon.com/comprehend/latest/dg/how-it-works.html

https://aws.amazon.com/comprehend/pricing/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Comprehend

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Comprehend++hands+on

***************************************************************************************************
## <a id="section-02"> </a> **2 - Amazon Forecast**

![Amazon Forecast](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Forecast_64.svg "Amazon Forecast")

**Definitions**

- Forecast business outcomes easily and accurately using machine learning
- Forecast 10,000 time series for 2 months with the AWS Free Tier
- Scale operations by forecasting millions of items, using the same technology as Amazon.com.
- Optimize inventory and reduce waste with accurate forecasts at a granular level.
- Improve capital utilization and make long-term decisions with more confidence.
- Increase customer satisfaction with optimal staffing to meet varying demand levels.

**Cheat Sheets**

**References:**

https://aws.amazon.com/forecast/

https://aws.amazon.com/forecast/features/

https://aws.amazon.com/forecast/pricing/

https://aws.amazon.com/forecast/embedded-solutions/

https://aws.amazon.com/forecast/resources/?amazon-forecast-whats-new.sort-by=item.additionalFields.postDateTime&amazon-forecast-whats-new.sort-order=desc

https://aws.amazon.com/forecast/customers/

https://aws.amazon.com/forecast/partners/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Forecast

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Forecast++hands+on

***************************************************************************************************
## <a id="section-03"> </a> **3 - Amazon Fraud Detector**

![Amazon Fraud Detector](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Fraud-Detector_64.svg "Amazon Fraud Detector")

**Definitions**

### **What is Amazon Fraud Detector?**

- Amazon Fraud Detector is a fully managed fraud detection service that automates the detection of potentially fraudulent activities online. 
- These activities include unauthorized transactions and the creation of fake accounts. Amazon Fraud Detector works by using machine learning to analyze your data. It does this in a way that builds off of the seasoned expertise of more than 20 years of fraud detection at Amazon.

- You can use Amazon Fraud Detector to build customized fraud-detection models, add decision logic to interpret the model’s fraud evaluations, and assign outcomes such as pass or send for review for each possible fraud evaluation. With Amazon Fraud Detector, you don't need machine learning expertise to detect fraudulent activities.

- To get started, collect and prepare fraud data that you collected at your organization. 
- Amazon Fraud Detector then uses this data to train, test, and deploy a custom fraud detection model on your behalf. As a part of this process, Amazon Fraud Detector uses machine learning models that have learned patterns of fraud from AWS and Amazon’s own fraud expertise to evaluate your fraud data and generate model scores and model performance data. 
- You configure decision logic to interpret the model’s score and assign outcomes for how to deal with each fraud evaluation.

- Detect online fraud faster with machine learning
- Up to 30,000 fraud predictions
    - per month free with the AWS Free Tier
- Build, deploy, and manage fraud detection models without previous machine learning (ML) experience.
- Gain insights from your historical data, plus 20+ years of Amazon experience, to construct an accurate, customized fraud detection model.
- Start detecting fraud immediately, easily enhance models with customized business rules, and deploy results to generate critical predictions.

**Cheat Sheets**

**References:**

https://aws.amazon.com/fraud-detector/

https://docs.aws.amazon.com/frauddetector/latest/ug/what-is-frauddetector.html

https://aws.amazon.com/fraud-detector/features/

https://aws.amazon.com/fraud-detector/pricing/

https://aws.amazon.com/fraud-detector/faqs/

https://aws.amazon.com/fraud-detector/resources/?blog-posts-cards.sort-by=item.additionalFields.createdDate&blog-posts-cards.sort-order=desc

https://aws.amazon.com/fraud-detector/customers/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Fraud+Detector

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Fraud+Detector+hands+on

***************************************************************************************************
## <a id="section-04"> </a> **4 - Amazon Kendra**

![Amazon Kendra](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Kendra_64.svg "Amazon Kendra")

**Definitions**

- Amazon Kendra is a highly accurate and intelligent search service that allows your users to search unstructured and structured data using natural language processing and advanced search algorithms. 
- It returns specific answers to questions, giving users an experience that's close to interacting with a human expert. 
- It is highly scalable and capable of meeting performance demands, tightly integrated with other AWS services such as Amazon S3 and Amazon Lex, and offers enterprise-grade security.
- For information on Amazon Kendra and Amazon Kendra Intelligent Ranking API operations, see the API reference documentation.
- Amazon Kendra users can ask the following types of questions, or queries:
    - Factoid questions—Simple who, what, when, or where questions, such as Where is the nearest service center to Seattle? Factoid questions have fact-based answers that can be returned in the form of a single word or phrase. The answer is retrieved from a FAQ or from your indexed documents.
    - Descriptive questions—Questions where the answer could be a sentence, passage, or an entire document. For example, How do I connect my Echo Plus to my network? or How do I get tax benefits for lower income families?.
    - Keyword and natural language searches—Questions that not only include keywords to search on but also complex, conversational questions. This includes questions where the intended meaning isn't always clear. For example, keynote address. Since 'address' can often have several meanings, Amazon Kendra can infer the user's intended meaning behind the search query to return relevant information. Amazon Kendra uses deep learning models to handle this kind of query.

### **Benefits of Amazon Kendra**

**Amazon Kendra has the following benefits:**
- **Accuracy—Unlike traditional** search services that use keyword searches where results are based on basic keyword matching and ranking, Amazon Kendra attempts to understand the context of the question. Amazon Kendra searches across your data and goes beyond traditional search to return the most relevant word, snippet, or document for your query. Amazon Kendra uses machine learning to improve search results over time.
- **Simplicity—Amazon** Kendra provides a console and API for managing your documents that you want to search. You can use a simple search API to integrate Amazon Kendra into your client applications, such as websites or mobile applications.
- **Connectivity—Amazon** Kendra can connect to third-party data repositories or data sources such as Microsoft SharePoint. You can easily index and search your documents using your data source.
- **User access** control—Amazon Kendra delivers highly secure enterprise search for your search applications. Your search results reflect the security model of your organization. Search results can be filtered based on the user or their group access to documents. Customers are responsible for authenticating and authorizing user access.

### **Amazon Kendra Developer Edition**
The Amazon Kendra Developer Edition provides all of the features of Amazon Kendra at a lower cost. It includes a free tier that provides 750 hours of use. The Developer Edition is ideal to explore how Amazon Kendra indexes your documents, to try out features, and to develop applications that use Amazon Kendra.

The Developer Edition provides the following:
- Up to 5 indexes with up to 5 data sources each.
- 10,000 documents or 3 GB of extracted text.
- Approximately 4,000 queries per day or 0.05 queries per second.
- Runs in 1 availability zone (AZ)—see Availability Zones (data centers in AWS regions)

You should not use the Developer Edition for a production application. The Developer Edition doesn't provide any guarantees of latency or availability.

### **Amazon Kendra Enterprise Edition**
Use Amazon Kendra Enterprise Edition when you want to index your entire enterprise document library or for when your application is ready for use in a production environment.

The Enterprise Edition provides the following:
- Up to 5 indexes with up to 50 data sources each.
- 100,000 documents or 30 GB of extracted text.
- Approximately 8,000 queries per day or 0.1 queries per second.
- Runs in 3 availability zones (AZ)—see Availability Zones (data centers in AWS regions)

You can increase this quota using the Service Quotas console.

### **Pricing for Amazon Kendra**
- You can get started for free with the Amazon Kendra Developer Edition that provides usage of up to 750 hours for the first 30 days. After your trial expires, you are charged for all provisioned Amazon Kendra indexes, even if they are empty and no queries are executed. After the trial expires, there are additional charges for scanning and syncing documents using the Amazon Kendra data sources.

- Up to 750 hours of free usage for 30 days
with the AWS Free Tier

**Cheat Sheets**

**References:**

https://aws.amazon.com/kendra/

https://aws.amazon.com/kendra/pricing/

https://aws.amazon.com/kendra/features/

https://aws.amazon.com/kendra/connectors/

https://aws.amazon.com/kendra/intelligent-ranking-pricing/

https://aws.amazon.com/kendra/resources/?blog-cards.sort-by=item.additionalFields.createdDate&blog-cards.sort-order=desc

https://aws.amazon.com/kendra/faqs/

https://aws.amazon.com/kendra/customers/

**Videos**

https://youtu.be/Xj_d2eX4nTY

**Hands On**

***************************************************************************************************
## <a id="section-05"> </a> **5 - Amazon Lex**

![Amazon Lex](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Lex_64.svg "Amazon Lex")

**Definitions**

- A service that can help you build conversational interfaces using voice and text.
- Uses automatic speech recognition (ASR) to convert speech to text.
- Uses natural language understanding (NLU) for recognizing the intent of the text.
- Provides highly-engaging user experiences and lifelike conversational interactions.
- Gets more intelligent over time by using deep learning.

### **Common Use Cases**
- AI Chatbots
- Informational bots
- Enterprise Productivity bots
- Voice Assistants

### **Concepts**

- Bots
    - Performs automated tasks such as ordering food or booking flights.
    - Supports multiple intents – for example, a bot can book a reservation or may choose to cancel it.

- Intent
    - A set of actions given to a bot by a user.
    - Intent name
        - A description for the intent (e.g. ‘BookFlights’, ‘OrderFood’)
    - Sample utterances
        - Describes the tone of the intent.
    - How to fulfill the intent
        - Describes the method of fulfilling an intent.
        - Deeply integrates with AWS Lambda to fulfill the intent.
- Slot
    - An optional parameter used as a part of the intent configuration.
    - Slot type
        - You can create a custom or built-in slot type.
        - Each slot type should have a unique name within an AWS account.

### **Pricing**
- Pay-as-you-go payment model
- $0.004 per voice request
- $0.00075 per text request
- 10,000 text and 5,000 speech requests free for 12 months
    - with the AWS Free Tier 


**Cheat Sheets**

https://tutorialsdojo.com/amazon-lex/

**References:**

https://aws.amazon.com/lex/?nc=sn&loc=0

https://aws.amazon.com/lex/faqs/

https://docs.aws.amazon.com/lex/latest/dg/how-it-works.html

https://aws.amazon.com/lex/pricing/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Lex

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Lex+hands+on

***************************************************************************************************
## <a id="section-06"> </a> **6 - Amazon Polly**

![Amazon Polly](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Polly_64.svg "Polly")

**Definitions**

- A text-to-speech (TTS) service
- Uses advanced deep learning technologies to convert text into natural, lifelike speech
- It supports saving text into MP3, OGG, and PCM file formats.
- Offers Standard and Neural TTS (NTTS)

### Common use cases
- Increase customer engagement
- Language learning applications
- Helps visually impaired individuals to consume digital content
- Testing in-game dialogs
- Voice response


### **Concepts**

- Speech Synthesis Markup Language (SSML)
    - Uses XML-based tags to modify different aspects of the text-to-speech output.
    - Can control pitch, speaking style, speech rate, and volume.
- Standard TTS
   -  Concatenates short speech snippets together.
   -  Limited in terms of producing different speaking styles.
- Neural TTS
    - Produces higher quality speech output than Standard TTS.
    - Neural TTS supports two speaking styles:
       - Conversational
       - Newscaster
- Speech Mark
    -  Refers to the metadata that describes the synthesized speech
    -  Speech Mark has four types:
       -  Sentence
       -  Word
       -  Viseme
       -  SSML

### **Features**

- Amazon Polly accepts plain text, UTF-8, and SSML as inputs.
- Pronounces out abbreviations and acronyms
- Interprets date/time and unit of measurements.
- Homograph disambiguation 
    - For example,  “St.” can be read as ”saint” or “street.” Amazon Polly is capable of identifying their difference depending on a given context.

- Custom lexicon
    - Supports customizing the pronunciation of words uncommon to the selected language.


### **Pricing**

- Standard TTS
- $4.00 per 1 million characters
- Neural TTS
- $16.00 per 1 million characters
- With the AWS Free Tier
    - Get 5 million characters free per month for 12 months

**Cheat Sheets**

https://tutorialsdojo.com/amazon-polly/

**References:**

https://aws.amazon.com/polly/?nc=sn&loc=1

https://aws.amazon.com/polly/faqs/

https://aws.amazon.com/polly/features/

https://docs.aws.amazon.com/polly/latest/dg/how-text-to-speech-works.html

https://aws.amazon.com/polly/pricing/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Polly

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Polly+hands+on

***************************************************************************************************
## <a id="section-07"> </a> **7 - Amazon Rekognition**

![Amazon Rekognition](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Rekognition_64.svg "Amazon Rekognition")

**Definitions**

- A service that makes it easy to add powerful visual analysis to your applications.
- There are two services under Amazon Rekognition:
    - **Rekognition Image** lets you easily build powerful applications to search, verify, and organize millions of images.
    - **Rekognition Video** lets you extract motion-based context from stored or live stream videos and helps you analyze them.

### **Rekognition Image**
- An image recognition service that detects objects, scenes, and faces; extracts text, and many more.
- It also allows you to search and compare faces.
- The service uses deep neural network models to detect and label thousands of objects and scenes in your images.
- Common use cases:
    - Searchable Image Library
    - Face-Based User Verification
    - Sentiment Analysis
    - Facial Recognition
    - Image Moderation

- Rekognition Image currently supports the **JPEG and PNG** image formats. You can submit images either as an **S3 object (up to 15MB) or as a byte array (up to 5MB)**.
- Rekognition Image returns the bounding box for each face detected in an image along with its attributes such as sex, accessories, facial features, etc.
- Using the CompareFaces API, Rekognition Image lets you measure the likelihood that faces in two images are of the same person.

### **Rekognition Video**
- A video recognition service that detects activities; understands the movement of people in frame; and recognizes objects, celebrities, text, scenes, and many more in a video.
- Rekognition Video allows you also to index metadata like objects, text, activities, scene, celebrities, and faces that make video search easy.
- Common use cases
    - Search Index for video archives
    - Easy filtering of video for explicit and suggestive content
- Rekognition Video operations can analyze videos (up to 8GB) stored in Amazon S3 buckets. The video must be encoded using the H.264 codec. The supported file formats are **MPEG-4 and MOV**.
- With Rekognition Video, you can locate faces across a video and analyze face attributes.
- With the **Person Tracking** feature, you can also track each person within a shot and through the video across shots.
- Rekognition Video uses a **Kinesis Video Stream** as input, to process a video stream. The analysis results are output to a Kinesis data stream and finally read by your client application.

**Cheat Sheets**

https://tutorialsdojo.com/amazon-rekognition/

**References:**

https://aws.amazon.com/rekognition/?nc=sn&loc=1

https://docs.aws.amazon.com/rekognition/latest/dg/what-is.html

https://aws.amazon.com/rekognition/faqs/

https://aws.amazon.com/rekognition/pricing/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Rekognition

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Rekognition+hands+on

***************************************************************************************************
## <a id="section-08"> </a> **8 - Amazon SageMaker**

![Amazon SageMaker](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-SageMaker_64.svg "Amazon SageMaker")

**Definitions**

- A fully managed service that allows data scientists and developers to easily build, train, and deploy machine learning models at scale.
- Provides built-in algorithms that you can immediately use for model training.
- Also supports custom algorithms through docker containers.
- One-click model deployment.

### **Concepts**

- Hyperparameters
    - It refers to a set of variables that controls how a model is trained.
    - You can think of them as “volume knobs” that you can tune to acquire your model’s objective.

- Automatic Model Tuning
    - Finds the best version of a model by automating the training job within the limits of the hyperparameters that you specified.

- Training
    - The process where you create a machine learning model.

- Inference
    - The process of using the trained model to make predictions.

- Local Mode
    - Allows you to create and deploy estimators to your local machine for testing.
    - You must install the Amazon SageMaker Python SDK on your local environment to use local mode.

- Common Training Data Formats For Built-in Algorithms:
    - CSV
    - Protobuf RecordIO
    - JSON
    - Libsvm
    - JPEG
    - PNG

Input modes for transferring training data

- File mode
    - Downloads data into the SageMaker instance volume before model training commences.
    - Slower than pipe mode
    - Used for Incremental training

- Pipe mode
    - Directly stream data from Amazon S3 into the training algorithm container.
    - There’s no need to procure large volumes to store large datasets.
    - Provides shorter startup and training times.
    - Higher I/O throughputs
    - Faster than File mode.
    - You MUST use protobuf RecordIO as your training data format before you can take advantage of the Pipe mode.


**Two methods of deploying a model for inference**

- Amazon SageMaker Hosting Services
    - Provides a persistent HTTPS endpoint for getting predictions one at a time.
    - Suited for web applications that need sub-second latency response.
- Amazon SageMaker Batch Transform
    - Doesn’t need a persistent endpoint
    - Get inferences for an entire dataset

**Optimization**

- Convert training data into a protobuf RecordIO format to make use of Pipe mode.
- Use Amazon FSx for Lustre to accelerate File mode training jobs.


### **Monitoring**

- You can publish SageMaker instance metrics to the CloudWatch dashboard to gain a unified view of its CPU utilization, memory utilization, and latency.
- You can also send training metrics to the CloudWatch dashboard to monitor model performance in real-time.
- Amazon CloudTrail helps you detect unauthorized SageMaker API calls.

### **Pricing**

- The building, training, and deploying of ML models are billed by the second, with no minimum fees and no upfront commitments.

**Cheat Sheets**

https://tutorialsdojo.com/amazon-sagemaker/

**References:**
https://aws.amazon.com/sagemaker/?nc=sn&loc=1

https://aws.amazon.com/sagemaker/faqs/

https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html

https://aws.amazon.com/sagemaker/pricing/

**Videos**

https://www.youtube.com/results?search_query=Amazon+SageMaker

**Hands On**

https://www.youtube.com/results?search_query=Amazon+SageMaker+hands+on

***************************************************************************************************
## <a id="section-09"> </a> **9 - Amazon Textract**

![Amazon Textract](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Textract_64.svg "Amazon Textract")

**Definitions**

- A fully managed document analysis service for detecting and extracting information from scanned documents.
- Returns extracted data as key-value pairs (e.g., Name: John Doe)
- Supports virtually any type of documents
- Can detect text written in Standard English alphabet and ASCII symbols.

### Common Use Cases:

- Building search indexes
- Importing documents into a business application
- Building automated document processing solutions
- Text extraction for Natural Language Processing (NLP) Applications
- Maintaining document compliance

### Concepts

- Amazon Textract returns a confidence score for each identified element, which indicates the probability that a given prediction is correct.
- A low-confidence score can be rerouted to Amazon Augmented AI (A2I) for further human review.
- The asynchronous operation allows you to process multipage PDF documents.
- Detect Document Text API
    - Uses optical character recognition (OCR) technology to extract printed text and handwriting from a document.
- Analyze Document API
    - Extracts printed text, handwriting, and other data from tables and key-value pairs from forms.

### **Pricing**
- You only pay for what you use.
- Charges vary for Detect Document Text API and Analyze Document API, with the latter being the more expensive.


**Cheat Sheets**

https://tutorialsdojo.com/amazon-textract/

**References:**

https://docs.aws.amazon.com/textract/latest/dg/what-is.html

https://docs.aws.amazon.com/textract/latest/dg/textract-best-practices.html

https://aws.amazon.com/blogs/machine-learning/using-amazon-textract-with-amazon-augmented-ai-for-processing-critical-documents/

**Videos**

https://www.youtube.com/results?search_query=Amazon+Textract

**Hands On**

https://www.youtube.com/results?search_query=Amazon+Textract+hands+on

***************************************************************************************************
## <a id="section-10"></a> **10 - Amazon Transcribe**

![Amazon Transcribe](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Transcribe_64.svg "Amazon Transcribe")

**Definitions**

- A fully managed automatic speech recognition (ASR) service.
- Converts speech into text.
- It supports a wide variety of audio coding formats such as **WAV, MP3, MP4, FLAC, AMR, AMR-WB, Ogg, and WebM.**
- It can process batch and streaming transcriptions.

**Common Use Cases**

- Transcribing customer calls
- Meeting transcription
- Closed captioning
- Generating metadata to create a searchable archive

### **Concepts**

- A confidence score is between 0 and 100, indicating the probability that a given prediction is correct.
- Low-fidelity (lo-fi) is a term used to describe audio recordings that exhibit poor sound quality. The term high-fidelity refers to high-quality audio recordings.
- Automatic content redaction
    - A process that censors sensitive information within the transcript output.
    - Replaces redacted information with the [PII] tag.

### **Features**

- Custom Vocabulary
    - Helps improve accuracy for content that has business-specific terms such as medical or legal terms.
- Vocabulary Filtering 
    - Allows you to create a list of words to filter from the transcript.
    - Useful for blocking profanities.
- Multiple speaker recognition
    - Supports identifying up to a maximum of ten speakers.
- Capable of transcribing low-fidelity and high-fidelity audio files.
- Uses machine learning to provide punctuation and grammatical formatting, making the transcription output immediately usable.
- It adds timestamps to every word, making it easier to use for movie subtitles.
- Includes confidence scores at each result so you can easily pinpoint the sections where further editing is required.
- Transcribe Medical can automatically identify Protected Health Information (PHI). Amazon Transcribe Medical is a HIPAA-eligible automatic speech recognition service.


### **Pricing**

- Charges batch and streaming transcription jobs at a monthly rate of $0.0004 per second.
- Billed in 1-second increments
- Minimum request charge of 15 seconds.

**Cheat Sheets**

https://tutorialsdojo.com/amazon-transcribe/

**References:**

https://aws.amazon.com/transcribe/faqs/

https://aws.amazon.com/transcribe/features/

https://docs.aws.amazon.com/transcribe/latest/dg/how-it-works.html

https://aws.amazon.com/transcribe/pricing/

**Videos**

**Hands On**
***************************************************************************************************
## <a id="section-11"></a> **11 - Amazon Translate**

![Amazon Translate](../images/Architecture-Service-Icons_01312022/Arch_Machine-Learning/64/Arch_Amazon-Translate_64.svg "Amazon Translate")

**Definitions**

- A Neural Machine Translation service that provides fluent translation with higher accuracy than traditional statistical and rule-based translation models.
- Powered by deep learning models that deliver fast, accurate, and affordable translation between supported languages.
- Supports batch translation, real-time, and on-demand translations.


**Common Use Cases**

- Language localization
- Translating content for text analytics
- Cross-lingual communication


### **Concepts**

- Amazon Translate uses a Translation Model that consists of two (2) components:
    - Encoder
        - Read a source text one word at a time.
        - Creates a semantic representation of each word.
    - Decoder
        - Uses the constructed semantic representation of the encoded text and translates it to the target language one word at a time.
        - The decoder also uses a method called the Attention mechanism to translate obscure words or phrases correctly.
- When Automatic Language Detection is enabled, Amazon Translate uses Amazon Comprehend on the backend to automatically detect the language used in the source text.


### **Features**

- Broad Language Coverage
- Neural-Network Based
    - Produces high-quality translations by utilizing deep learning technologies.
- Customized Machine Translation
    - Enables you to tailor your translations to suit domain-specific terminologies.
    - Useful for changing the tone, style, and word choices for the translated text.
- Secure Machine Translation
    - Communications between Amazon Translate and your application is SSL-protected.

### **Pricing**

- Standard Translation
    - Billed for $15.00 per million characters
- Active Custom Translation
    - Billed for $60.00 per million characters

**Cheat Sheets**

https://tutorialsdojo.com/amazon-translate/

**References:**

https://aws.amazon.com/translate/

https://aws.amazon.com/translate/faqs/

https://docs.aws.amazon.com/translate/latest/dg/what-is.html

https://aws.amazon.com/translate/details/

https://aws.amazon.com/translate/pricing/

**Videos**

https://youtu.be/ymbYmHz8B8E

https://www.youtube.com/results?search_query=Amazon+Translate


**Hands On**

https://www.youtube.com/results?search_query=Amazon+Translate+hands+on