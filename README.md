# DataChatBot
In this project, We will create a chatbot for pdf file using Flask, a popular web framework, and LangChain, another popular framework for working with large language models (LLMs). The chatbot  We develop will not just interact with users through text but also comprehend and answer questions related to the content of a specific document.

**Step1** : pip install -r requirements.txt


**Step2**: In this project, you do not need to specify your own Watsonx_API and Project_id. Detailed instructions and further information are available in this [tutorial](https://medium.com/the-power-of-ai/ibm-watsonx-ai-the-interface-and-api-e8e1c7227358). 

**Chat Bot Demo:**

![image](https://github.com/user-attachments/assets/13022027-2f8e-4dae-9466-f6dff4ce4f4a)

=======
## How to get watsonx API key and Project ID

Here, we initialize a language model and its embeddings. Here's a brief description of each section of the script:

- API and Project ID: Watsonx_API and Project_id are variables storing the API key and project ID required to access IBM's cloud services.


- WatsonX LLM parameters Initialization: Inside the function, a dictionary named params is created, which holds various parameters like maximum and minimum number of tokens to generate, temperature (controlling randomness), and others for configuring the generation behavior of the language model.

- Credentials: A dictionary named credentials is defined with the URL of IBM's cloud service and the API key to authenticate requests to the service.
- LLM Initialization: A model object, `LLAMA2_model`, is created using the Model class, which is initialized with a specific model ID, credentials, parameters, and project ID. Then, an instance of WatsonxLLM is created with `LLAMA2_model` as an argument, initializing the language model hub `llm_hub`.


We also initialize embeddings. The embeddings are used to represent text data in a form that machines can understand. They convert human-readable text into numbers (vectors) that capture the semantic meaning of the text.

- The embeddings are initialized using a class called `HuggingFaceInstructEmbeddings` pre-trained model named `sentence-transformers/all-MiniLM-L6-v2` list of leaderboard of embeddings are available [here](https://huggingface.co/spaces/mteb/leaderboard). This embedding model has shown a good balance in both performance and speed.

## Get Your Watsonx API and Project ID
Since watsonx is an IBM Cloud service, credentials such as an API key and a project ID are required when accessing from the outside. 

To access the credentials, we've provided a special code for you to claim a USD 200 credit on IBM Cloud at no charge! Here's how to get started:
1. **IBM Cloud Trial Access:**
- Proceed to the "IBM Cloud Trial" section for the unique code and detailed instructions.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0XPBEN/ezgif.com-video-to-gif-converted.gif)
- Follow these instructions to sign up for a non-expiring Lite account at IBM Cloud, which includes the USD 200 credit.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0XPBEN/ezgif.com-video-to-gif-converted%20%281%29.gif)
2. **Create Your Watsonx Project:**
- Sign in to [IBM watsonx](https://dataplatform.cloud.ibm.com/registration/stepone?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-test1_v1_1702536549&context=wx&apps=data_science_experience%2Cwatson_data_platform%2Ccos) and [create a project](https://dataplatform.cloud.ibm.com/projects/?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-test1_v1_1702536549&context=wx).
![Getting IBM watsonx project ID](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0PPIEN/createProject.gif)
- Inside your project on watsonx, navigate to `Manage` > `General` to find your project ID for your later use.
![Create a project ID](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0XPBEN/id.gif)
3. **Associate Watson Machine Learning Service:**
After you create a project, you can go to the project’s `Manage` tab > select the `Services and integrations` page > click `Associate Service` > add the `Watson Machine Learning` service to it.
![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0PPIEN/associate.gif)
4. **Generate IBM Cloud User API Key:**
Lastly, you can follow the below demonstration to create/get your [IBM Cloud user API key](https://cloud.ibm.com/iam/apikeys?utm_source=skills_network&utm_content=in_lab_content_link&utm_id=Lab-test1_v1_1702536549). Be sure to write your API key down somewhere right after you create it, because you won’t be able to see it again!

![Getting IBM cloud user API key](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-GPXX0PPIEN/ezgif.com-video-to-gif.gif)
>>>>>>> 8110cc6 (Files regarding the DataChatBot)
>>>>>>>
>>>>>>> ![image](https://github.com/user-attachments/assets/45185833-973f-4952-9763-de8fddad6e17)

